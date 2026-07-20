# Kapitel 15 – Large Language Models und ihre Programmierung

{{ progress(15) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was ein **Large Language Model (LLM)** ist und wie es im Kern funktioniert
- Warum ein LLM „nur das nächste Wort vorhersagt" – und wieso das so mächtig ist
- Was **Parameter, Kontextfenster, Tokens und Temperatur** bedeuten
- Warum LLMs **halluzinieren** und was das für die Praxis heißt
- Wie man LLMs „programmiert" – nämlich mit **Sprache (Prompts)** statt Code
</div>

---

## 15.1 Was ist ein Large Language Model?

Ein **Large Language Model** ist ein sehr großes, mit riesigen Textmengen trainiertes neuronales Netz, das menschliche Sprache verstehen und erzeugen kann. „Large" bezieht sich auf die enorme Zahl an **Parametern** (Milliarden interner Stellschrauben) und die gewaltigen **Trainingsdaten** (großer Teil des öffentlichen Internets, Bücher, Code …).

Die Modelle hinter **Microsoft Copilot** (aus der GPT-Familie, Kap. 16) sind solche LLMs.

---

## 15.2 Das Kernprinzip: das nächste Wort vorhersagen

So verblüffend die Ergebnisse wirken – im Kern macht ein LLM **eine** Sache: Es sagt das **wahrscheinlichste nächste Wort** (genauer: Token) voraus, immer und immer wieder.

```mermaid
flowchart LR
    A([Der Himmel ist ...]) --> B([Modell berechnet Wahrscheinlichkeiten])
    B --> C([blau: 71% · bewölkt: 12% · hoch: 4% ...])
    C --> D([wählt Wort]) --> E([hängt es an, wiederholt])
```

Das Modell erzeugt Text **Wort für Wort**: Es nimmt den bisherigen Text, berechnet für alle möglichen nächsten Wörter eine Wahrscheinlichkeit, wählt eines aus, hängt es an – und beginnt von vorn.

!!! info "Warum das ausreicht für 'Intelligenz'"
    Man könnte meinen, „nur das nächste Wort raten" sei trivial. Aber um verlässlich das *richtige* nächste Wort zu wählen, muss das Modell Grammatik, Fakten, Logik und Stil **implizit** aus den Trainingsdaten gelernt haben. Aus dieser einen einfachen Aufgabe – konsequent im Riesenmaßstab – entstehen die erstaunlichen Fähigkeiten. Es ist **statistische Mustervorhersage**, kein Denken.

---

## 15.3 Wichtige Begriffe verstehen

| Begriff | Bedeutung | Praktische Auswirkung |
|---|---|---|
| **Token** | Wortbaustein (ca. 0,75 Wörter) | Länge/Kosten werden in Tokens gemessen |
| **Parameter** | gelernte interne Stellschrauben | mehr = i. d. R. leistungsfähiger |
| **Kontextfenster** | wie viel Text das Modell „gleichzeitig sieht" | begrenzt, wie viel du eingeben kannst |
| **Temperatur** | Grad an Zufall/Kreativität | niedrig = präzise, hoch = kreativ |
| **Training** | einmaliges Lernen aus Daten | danach ist Wissen „eingefroren" |

### Das Kontextfenster – eine wichtige Grenze

Ein LLM kann nur eine **begrenzte Menge Text** auf einmal berücksichtigen (das Kontextfenster). Alles, was darüber hinausgeht, „vergisst" es.

!!! example "Praktische Folge"
    Gibst du Copilot ein sehr langes Dokument, kann es sein, dass frühe Passagen weniger Gewicht bekommen. Abhilfe: in **Abschnitte** aufteilen, gezielt fragen, oder erst zusammenfassen lassen und dann auf der Zusammenfassung weiterarbeiten.

### Wissensstichtag

Das Wissen eines LLM ist zum Zeitpunkt des Trainings **eingefroren**. Neuere Ereignisse kennt es nur, wenn es (wie Copilot per Websuche oder RAG, Kap. 5) zusätzliche, aktuelle Quellen bekommt.

---

## 15.4 Warum LLMs halluzinieren

Weil ein LLM immer das **plausibelste** nächste Wort wählt, kann es Inhalte erzeugen, die **flüssig und überzeugend** klingen, aber **sachlich falsch** sind. Das nennt man **Halluzination**.

!!! warning "Der zentrale Merksatz"
    Ein LLM optimiert auf **Plausibilität**, nicht auf **Wahrheit**. Es „weiß" nicht, ob etwas stimmt – es erzeugt, was statistisch am besten passt. Erfundene Quellen, falsche Zahlen oder nicht existierende Paragraphen sind typische Halluzinationen. Deshalb gilt ausnahmslos: **Fakten prüfen.**

Halluzinationen werden wahrscheinlicher, wenn:

- nach sehr spezifischen Fakten/Zahlen gefragt wird, die selten im Training vorkamen,
- die Frage außerhalb des Trainingswissens liegt (zu neu, zu speziell),
- der Prompt vage ist und das Modell „auffüllen" muss.

Gegenmittel: **Quellen mitgeben** (RAG/Dokument-Upload), um **Belege bitten**, Ergebnisse **gegenprüfen**.

---

## 15.5 LLMs „programmieren" – mit Sprache

Der große Bruch: Man steuert LLMs nicht mit Programmcode, sondern mit **natürlicher Sprache**. Der Prompt **ist** das Programm.

| Klassische Programmierung | LLM „programmieren" |
|---|---|
| Code in einer Programmiersprache | Anweisung in natürlicher Sprache |
| exakte, feste Logik | flexible, statistische Antwort |
| Entwickler:innen nötig | jede:r kann es |

Genau deshalb ist **Prompt Engineering** (Kap. 14) die entscheidende Fähigkeit: Es ist die „Programmiersprache" der LLMs.

**Copilot-Prompt zum Ausprobieren:**

```text
Erkläre in einfachen Worten, warum ein Sprachmodell manchmal falsche, aber
überzeugend klingende Antworten gibt. Nenne anschließend drei konkrete
Maßnahmen, mit denen ich als Nutzer:in dieses Risiko verringere.
```

---

## Zusammenfassung

- Ein **LLM** ist ein riesiges, aus Textmengen trainiertes Netz; Copilot beruht auf GPT-LLMs.
- Es sagt im Kern nur das **nächste Wort** voraus – daraus entstehen im Großmaßstab erstaunliche Fähigkeiten.
- Wichtige Begriffe: **Token, Parameter, Kontextfenster, Temperatur**; Wissen ist zum Training **eingefroren**.
- LLMs **halluzinieren**, weil sie auf **Plausibilität statt Wahrheit** optimieren – deshalb prüfen.
- Man „programmiert" LLMs mit **Sprache** – deshalb ist Prompt Engineering die Schlüsselkompetenz.

---

## Kurzübungen

{{ task(file="tasks/k15_01.yaml") }}

{{ task(file="tasks/k15_02.yaml") }}

{{ task(file="tasks/k15_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k15.yaml") }}
