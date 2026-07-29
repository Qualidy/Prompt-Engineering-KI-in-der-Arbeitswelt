# Kapitel 20 – Data-Mining

{{ progress(20) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **Data-Mining** ist und wie es sich von einfacher Statistik unterscheidet
- Die zentralen **Analysemuster**: Klassifikation, Clustering, Assoziation, Ausreißer, Prognose
- Ein anschauliches Beispiel: die **Warenkorbanalyse**
- Wie man Assoziationsregeln mit **Support, Confidence und Lift** liest (durchgerechnet)
- Der geordnete **Ablauf** eines Data-Mining-Projekts (CRISP-DM)
- Der Unterschied zwischen **Korrelation und Kausalität**
- Wie **Copilot in Excel** einfache Data-Mining-Fragen beantwortet – und wo Grenzen sind
</div>

---

## 20.1 Was ist Data-Mining?

**Data-Mining** bedeutet, in großen Datenmengen nach **verborgenen Mustern, Zusammenhängen und Regeln** zu „graben", die man vorher nicht kannte. Es geht nicht darum, eine bekannte Zahl abzulesen, sondern **Neues zu entdecken**.

!!! info "Abfrage vs. Entdeckung"
    „Wie viel Umsatz hatten wir im März?" ist eine **Abfrage** – die Antwort steht in den Daten. „Welche Kundengruppen kaufen zusammen welche Produkte und warum?" ist **Data-Mining** – hier sucht man Muster, die niemand vorgegeben hat. Data-Mining ist damit ein Kern der Analyse-Rolle von KI (Kap. 3).

---

## 20.2 Die zentralen Analysemuster

| Muster | Frage | Beispiel |
|---|---|---|
| **Klassifikation** | In welche Kategorie gehört das? | Kunde: kündigt / bleibt |
| **Clustering** | Welche Gruppen gibt es? | Kundensegmente entdecken |
| **Assoziation** | Was tritt gemeinsam auf? | „Wer A kauft, kauft auch B" |
| **Ausreißererkennung** | Was ist auffällig? | Betrug, Fehlbuchung |
| **Prognose** | Wie geht es weiter? | Absatz nächsten Monat |

Diese Muster bauen auf den ML-Grundlagen aus Kapitel 12 auf (überwacht/unüberwacht).

---

## 20.3 Beispiel: die Warenkorbanalyse

Das klassische Data-Mining-Beispiel ist die **Assoziationsanalyse** (Warenkorbanalyse): Welche Produkte werden häufig **zusammen** gekauft?

```mermaid
flowchart LR
    A([Millionen Kassenbons]) --> B([Muster suchen: was liegt zusammen im Korb?])
    B --> C([Regel: Windeln -> auch Bier])
    C --> D([Aktion: Platzierung, Angebote, Empfehlungen])
```

!!! example "Der berühmte 'Windeln-und-Bier'-Fall"
    Eine – oft erzählte – Analyse ergab, dass abends häufig **Windeln und Bier** zusammen gekauft wurden (vermutlich junge Väter). Ob die Geschichte exakt so stimmt, ist zweitrangig: Sie zeigt die Idee. **Handlungsfolge:** Produkte klug platzieren, Kombi-Angebote schnüren, Empfehlungen aussprechen („Kunden kauften auch …"). Genau dieses Prinzip steckt hinter Empfehlungssystemen im Online-Handel.

---

## 20.4 Korrelation ≠ Kausalität

Der wichtigste Denkfehler beim Data-Mining: aus einem **Zusammenhang** voreilig eine **Ursache** zu schließen.

!!! warning "Der klassische Trugschluss"
    Im Sommer steigen sowohl der **Speiseeis-Verkauf** als auch die Zahl der **Sonnenbrände**. Beide **korrelieren** – aber Eis verursacht keinen Sonnenbrand. Die gemeinsame Ursache ist das **warme Wetter**. Data-Mining findet **Korrelationen**; ob dahinter eine echte **Ursache-Wirkung** steckt, muss fachlich geprüft werden. Wer das verwechselt, trifft teure Fehlentscheidungen.

---

## 20.5 Assoziationsregeln lesen: Support, Confidence, Lift

Damit die Warenkorbanalyse aus Abschnitt 20.3 nicht bei einem Bauchgefühl bleibt, misst man jede Regel („Wer A kauft, kauft auch B") mit drei Kennzahlen. Rechnen wir es an einem kleinen Beispiel durch: **1.000 Kassenbons**, davon enthalten 200 **Kaffee**, 150 **Kuchen** und 120 **beides**.

| Kennzahl | Bedeutung | Rechnung | Ergebnis |
|---|---|---|---|
| **Support** | Wie oft tritt die Kombi überhaupt auf? | 120 / 1.000 | 12 % |
| **Confidence** | Wie oft folgt B, wenn A gekauft wird? | 120 / 200 | 60 % |
| **Lift** | Wie stark hängen A und B wirklich zusammen? | 0,60 / (150/1.000) | 4,0 |

So liest man die Zahlen: Die Regel „Kaffee → Kuchen" kommt in **12 %** aller Einkäufe vor (Support). Wer Kaffee kauft, nimmt in **60 %** der Fälle auch Kuchen (Confidence). Und der **Lift von 4,0** heißt: Kaffee-Käufer greifen **viermal so häufig** zu Kuchen wie ein durchschnittlicher Kunde. Ein Lift über 1 signalisiert einen echten positiven Zusammenhang – genau solche Regeln sind für Platzierung und Angebote interessant.

!!! warning "Häufiges Missverständnis: hohe Confidence ist nicht alles"
    Eine Confidence von 60 % klingt stark – kann aber täuschen. Wäre Kuchen ohnehin in 60 % **aller** Bons, brächte die Regel keine neue Erkenntnis: Der **Lift** läge bei 1,0 (kein Zusammenhang). Deshalb reicht Confidence allein nicht. Erst der **Lift** verrät, ob A und B wirklich zusammengehören oder ob B einfach nur ein Verkaufsschlager ist. Wer nur auf Confidence schaut, baut Aktionen auf Scheinmustern auf.

---

## 20.6 Der Ablauf eines Data-Mining-Projekts (CRISP-DM)

Data-Mining ist kein Knopfdruck, sondern ein **geordneter Prozess**. Der Industriestandard dafür heißt **CRISP-DM** (*Cross-Industry Standard Process for Data Mining*) und lässt sich in sechs Phasen fassen:

```mermaid
flowchart LR
    A([Geschäft verstehen]) --> B([Daten verstehen]) --> C([Daten aufbereiten])
    C --> D([Modellieren]) --> E([Bewerten]) --> F([Einsetzen])
    E --> A
```

Wichtig sind die **Ränder**: Am Anfang steht nicht die Technik, sondern die **Geschäftsfrage** („Was wollen wir wissen und wozu?"). Am Ende steht nicht das Modell, sondern der **produktive Einsatz** und die laufende Überprüfung. Der größte Zeitanteil liegt fast immer in **Datenbeschaffung und -aufbereitung** (Kap. 9 und 10) – die eigentliche Musteranalyse ist oft der kleinere Teil.

!!! info "Vertiefung: Warum der Kreislauf zurückführt"
    Der Pfeil von „Bewerten" zurück zu „Geschäft verstehen" ist kein Schönheitsfehler: Häufig zeigt die erste Auswertung, dass die Frage geschärft, andere Daten geholt oder das Ziel neu gefasst werden muss. Data-Mining ist damit **iterativ** – ähnlich dem iterativen Nachschärfen beim Prompt Engineering (Kap. 14). Wer nach dem ersten Durchlauf aufhört, verschenkt den größten Teil der Erkenntnis.

---

## 20.7 Data-Mining light mit Copilot in Excel

Für einfache Fragen brauchst du kein Data-Science-Team – **Copilot in Excel** liefert erste Erkenntnisse per Sprache:

| Aufgabe | Beispiel-Prompt |
|---|---|
| Trends erkennen | „Welche Trends zeigt diese Verkaufstabelle über 12 Monate?" |
| Gruppen bilden | „Fasse die Kunden nach Umsatzhöhe in 3 Gruppen zusammen." |
| Auffälligkeiten | „Welche Werte sind ungewöhnlich hoch oder niedrig?" |
| Zusammenhänge | „Gibt es einen Zusammenhang zwischen Rabatt und Absatzmenge?" |

**Beispiel-Prompt zum Ausprobieren:**

```text
Analysiere die markierte Verkaufstabelle: Nenne die drei auffälligsten Muster,
eine mögliche Erklärung je Muster und weise ausdrücklich darauf hin, wo es sich
nur um eine Korrelation und nicht um eine belegte Ursache handelt.
```

!!! tip "Copilot als Einstieg, nicht als Endpunkt"
    Copilot ist stark darin, **erste Hypothesen** zu liefern und dich auf interessante Stellen zu stoßen. Für belastbare, statistisch abgesicherte Aussagen (Signifikanz, echte Kausalität) braucht es echte Analyseverfahren und Fachwissen. Nutze Copilot, um **die richtigen Fragen** zu finden.

---

## Zusammenfassung

- **Data-Mining** entdeckt **unbekannte Muster** in großen Daten – mehr als bloßes Abfragen.
- Zentrale Muster: **Klassifikation, Clustering, Assoziation, Ausreißer, Prognose**.
- Die **Warenkorbanalyse** zeigt, wie aus Mustern konkrete Geschäftsaktionen werden.
- Assoziationsregeln misst man mit **Support, Confidence und Lift** – erst der **Lift** trennt echte Zusammenhänge von Scheinmustern.
- **CRISP-DM** gibt Data-Mining einen geordneten, iterativen Ablauf – von der Geschäftsfrage bis zum Einsatz.
- **Korrelation ist nicht Kausalität** – der wichtigste Denkfehler, den es zu vermeiden gilt.
- **Copilot in Excel** liefert schnelle Hypothesen; für belastbare Aussagen braucht es Fachverfahren.

---

## Kurzübungen

{{ task(file="tasks/k20_01.yaml") }}

{{ task(file="tasks/k20_02.yaml") }}

{{ task(file="tasks/k20_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k20.yaml") }}
