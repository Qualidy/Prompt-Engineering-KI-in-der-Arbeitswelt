# Kapitel 19 – Medienerstellung mit KI

{{ progress(19) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Welche **Medienarten** KI heute erzeugen kann: Text, Bild, Audio, Video, Präsentationen
- Wie **Bildgeneratoren** grundsätzlich funktionieren und wie man sie promptet
- Was **hinter der Bilderzeugung** steckt (Diffusion, vereinfacht) und wo ihre Grenzen liegen
- Wie du mit **Copilot** Präsentationen, Texte und Bildideen erstellst
- Welche **rechtlichen Fragen** (Urheberrecht, Kennzeichnung) zu beachten sind
- Wie du KI-Medien **qualitätssicher** und verantwortungsvoll einsetzt
</div>

---

## 19.1 Was KI heute erzeugen kann

**Generative KI** beschränkt sich längst nicht auf Text. Sie erstellt Inhalte in vielen Formaten:

| Medienart | Beispiel | Werkzeug (Beispiel) |
|---|---|---|
| Text | Berichte, E-Mails, Slogans | Copilot, ChatGPT |
| Bild | Illustrationen, Konzeptgrafiken | Copilot/Designer (DALL·E) |
| Präsentation | Foliensätze aus Text | Copilot in PowerPoint |
| Audio | Sprachausgabe, Musik | spezialisierte Tools |
| Video | Clips, Avatare | spezialisierte Tools |

Für den Büroalltag am relevantesten sind **Text, Präsentationen und Bilder** – alle direkt über Copilot bzw. den Microsoft Designer erreichbar.

---

## 19.2 Wie Bildgeneratoren funktionieren

Bild-KI (z. B. DALL·E, das in Microsoft-Produkten steckt) erzeugt Bilder aus einer **Textbeschreibung**. Vereinfacht: Das Modell hat aus Millionen **Bild-Text-Paaren** gelernt, wie Beschreibungen und Bildinhalte zusammenhängen, und setzt aus einem „Rauschen" schrittweise ein passendes Bild zusammen.

```mermaid
flowchart LR
    A([Textbeschreibung / Prompt]) --> B([Modell mit gelernten Bild-Text-Mustern])
    B --> C([erzeugtes Bild])
    C --> D([verfeinern durch präziseren Prompt])
    D --> B
```

**Ein guter Bild-Prompt beschreibt:**

| Element | Beispiel |
|---|---|
| Motiv | „ein moderner Büroarbeitsplatz" |
| Stil | „fotorealistisch" / „Flat-Illustration" |
| Stimmung/Licht | „hell, freundlich, Morgenlicht" |
| Perspektive | „Vogelperspektive", „Nahaufnahme" |
| Format | „Querformat, viel Freiraum links für Text" |

!!! example "Vom vagen zum präzisen Bild-Prompt"
    **Vage:** „ein Büro"
    **Präzise:** „Ein moderner, heller Büroarbeitsplatz mit Laptop und Pflanze, fotorealistisch, Morgenlicht, Querformat, ruhige Farben, viel Freiraum oben für eine Überschrift."
    Je konkreter Motiv, Stil und Bildaufbau, desto brauchbarer das Ergebnis.

---

## 19.3 Medien erstellen mit Copilot

**Präsentation aus Text (PowerPoint):**

```text
Erstelle eine Präsentation mit 7 Folien zum Thema "KI im Kundenservice".
Struktur: Titel, Problem, Lösung, 3 Vorteile, Beispiel, Fazit.
Pro Folie max. 4 Stichpunkte und ein Vorschlag für ein passendes Bildmotiv.
```

**Text mit passendem Stil:**

```text
Schreibe einen LinkedIn-Post (max. 120 Wörter), der unser neues KI-Projekt
vorstellt. Ton: professionell, aber begeistert. Ende mit einer Frage an die
Leser:innen.
```

**Bildidee entwickeln:**

```text
Ich brauche ein Titelbild für eine Schulung über Prompt Engineering.
Beschreibe 3 verschiedene Bildkonzepte, die ich in einem Bildgenerator
verwenden könnte – jeweils mit Stil, Motiv und Stimmung.
```

!!! tip "KI liefert den Rohentwurf, du den Feinschliff"
    KI-Medien sind selten sofort perfekt. Nutze sie als **schnellen ersten Entwurf** (Struktur der Folien, Bildidee, Textgerüst) und verfeinere gezielt. Das spart die mühsame „weiße Blatt"-Phase.

---

## 19.4 Recht und Kennzeichnung

!!! warning "Wichtige rechtliche Punkte"
    - **Urheberrecht der Eingaben:** Lade keine fremden, geschützten Bilder/Texte hoch, um sie „nachmachen" zu lassen.
    - **Rechte an den Ausgaben:** Die Rechtslage zu KI-generierten Werken ist teils ungeklärt und je nach Land unterschiedlich – für kommerzielle Nutzung genau prüfen.
    - **Kennzeichnungspflicht:** Der **EU AI Act** verlangt zunehmend, KI-generierte oder -manipulierte Inhalte **zu kennzeichnen** (Kap. 32).
    - **Persönlichkeitsrechte:** Keine realen Personen ohne Einwilligung darstellen (Deepfake-Problematik).

---

## 19.5 Qualität und Verantwortung

Bei KI-Medien sind typische Fehlerquellen zu beachten:

| Risiko | Beispiel | Gegenmittel |
|---|---|---|
| faktische Fehler im Text | falsche Zahl in Folie | gegenprüfen |
| unrealistische Bilddetails | „sechs Finger", falsche Logos | genau anschauen |
| Verzerrungen (Bias) | einseitige Darstellungen | bewusst gegensteuern (Kap. 31) |
| Marken-/Stilklau | fremder Look nachgeahmt | eigene Vorgaben nutzen |

**Copilot-Prompt zum Ausprobieren:**

```text
Erstelle die Gliederung (8 Folien) für eine Kundenpräsentation zu unserem
neuen Service. Markiere je Folie, welche Angabe ich unbedingt selbst auf
Richtigkeit prüfen muss.
```

---

## 19.6 Vom Rauschen zum Bild: der Diffusionsprozess

In Abschnitt 19.2 hieß es, das Modell setze „aus einem Rauschen schrittweise ein Bild zusammen". Dahinter steckt ein Verfahren namens **Diffusion**. Es lässt sich in zwei Richtungen verstehen:

- **Beim Training** nimmt man echte Bilder und fügt ihnen Schritt für Schritt **Rauschen** hinzu, bis nur noch ein zufälliges Pixelchaos übrig ist. Das Modell lernt dabei, diesen Vorgang **umzukehren**.
- **Bei der Erzeugung** startet das Modell mit reinem Rauschen und „entrauscht" es Schritt für Schritt – gelenkt durch deinen Text-Prompt, bis ein Bild entsteht, das zur Beschreibung passt.

```mermaid
flowchart LR
    A([reines Rauschen]) --> B([Schritt für Schritt entrauschen])
    B --> C([Prompt lenkt jeden Schritt])
    C --> D([fertiges Bild])
```

!!! info "Vertiefung: Warum die Verbindung von Text und Bild funktioniert"
    Damit ein Prompt das Entrauschen steuern kann, muss das Modell Sprache und Bildinhalte in einen **gemeinsamen Bedeutungsraum** übersetzt haben. Es hat aus Millionen Bild-Text-Paaren gelernt, dass das Wort „Sonnenuntergang" mit bestimmten Farben, Formen und Lichtstimmungen zusammenhängt. Das ist dieselbe Grundidee wie beim Sprachverstehen in Kap. 13 (NLP) – nur über zwei Medien hinweg. Deshalb wirken zusätzliche, konkrete Wörter im Prompt wie „Stellschrauben" für das Ergebnis.

---

## 19.7 Grenzen der Bild-KI und gezielte Feinsteuerung

Bild-KI ist beeindruckend, hat aber typische **Schwachstellen**, die man kennen sollte – sie folgen direkt aus der Funktionsweise (das Modell „malt" Wahrscheinliches, es „versteht" nichts):

| Schwäche | Warum | Umgang |
|---|---|---|
| Text im Bild oft fehlerhaft | Buchstaben sind für das Modell nur Formen | Beschriftung nachträglich selbst setzen |
| Hände, Zähne, Symmetrie | seltene, komplexe Detailmuster | Bild genau prüfen, neu generieren |
| Logos/Marken verfälscht | keine exakte Reproduktion | echte Logos separat einfügen |
| „Durchschnittslook" | Modell mittelt Gelerntes | Stil und Details präzise vorgeben |

Zur **Feinsteuerung** hilft es, nicht nur zu sagen, was ins Bild soll, sondern auch, was **nicht** – und Ausgabeparameter wie Format explizit zu nennen.

!!! example "Copilot-Dialog: drei Bildkonzepte vergleichen"
    **Prompt:**
    ```text
    Erfinde ein Titelbild-Motiv für eine Schulung zu Prompt Engineering.
    Beschreibe drei Varianten, jeweils mit Stil, Motiv, Stimmung und einem
    Hinweis, was NICHT im Bild sein soll (z. B. Text, Logos).
    ```
    **Beispiel-Output (gekürzt):**
    ```text
    1) Flat-Illustration: Person am Laptop, Sprechblase mit Zahnrad, ruhige Blautöne,
       freundlich. Kein Text, keine Markenlogos.
    2) Fotorealistisch: heller Schreibtisch, Notizzettel mit Pfeilen, Morgenlicht,
       viel Freiraum oben. Keine lesbaren Buchstaben, keine Gesichter.
    3) Minimalistisch: einzelnes Glühbirnen-Symbol aus Wortwolke, dunkler Hintergrund,
       fokussiert. Kein Fließtext, kein Firmenlogo.
    ```
    Diese Konzepte kannst du direkt in einen Bildgenerator übernehmen – die „Kein-Text/kein-Logo"-Hinweise beugen den typischen Fehlern vor.

!!! warning "Häufiges Missverständnis: ‚Die KI sucht ein passendes Foto heraus'"
    Ein Bildgenerator **durchsucht keine Datenbank** und fügt auch keine Bildschnipsel zusammen. Er erzeugt jedes Bild **neu** aus Rauschen. Das erklärt zweierlei: Erstens gibt es keine „Quelle", auf die man sich berufen kann. Zweitens ist das Ergebnis nicht zufällig „von jemandem geklaut" – wohl aber kann es gelernten Stilen ähneln, was die urheber- und persönlichkeitsrechtlichen Fragen aus Abschnitt 19.4 aufwirft.

---

## Zusammenfassung

- Generative KI erstellt **Text, Bild, Präsentation, Audio, Video** – im Büro v. a. Text, Folien, Bilder.
- **Bildgeneratoren** brauchen präzise Prompts (Motiv, Stil, Stimmung, Perspektive, Format).
- Technisch steckt dahinter **Diffusion**: aus Rauschen wird per Prompt schrittweise ein neues Bild – es wird nichts „herausgesucht".
- Typische **Grenzen** (Text im Bild, Hände, Logos) folgen aus der Funktionsweise – gezielt gegensteuern und prüfen.
- **Copilot** liefert schnelle Rohentwürfe – der Feinschliff und die Faktenprüfung bleiben bei dir.
- Beachte **Urheberrecht, Kennzeichnungspflicht (EU AI Act) und Persönlichkeitsrechte**.

---

## Kurzübungen

{{ task(file="tasks/k19_01.yaml") }}

{{ task(file="tasks/k19_02.yaml") }}

{{ task(file="tasks/k19_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k19.yaml") }}
