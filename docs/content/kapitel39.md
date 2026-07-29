# Kapitel 39 – KI-Strategie und strategisches KI-Management

{{ progress(39) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was eine **KI-Strategie** ist und warum „einfach mal machen" scheitert
- Die zentralen **Bausteine** einer KI-Strategie
- Wie man Use Cases **priorisiert** und in eine **Roadmap** bringt
- Die Rolle von **Governance, Kompetenzaufbau und Kultur**
- Die **Make-or-Buy-Entscheidung**: selbst bauen, kaufen oder anpassen
- Wie du mit **Copilot** eine erste Strategie-Skizze erstellst
</div>

---

## 39.1 Warum es eine Strategie braucht

Viele Unternehmen starten mit **verstreuten KI-Experimenten** ohne roten Faden. Das führt zu Insellösungen, doppelter Arbeit und Frust. Eine **KI-Strategie** gibt Richtung: Wo wollen wir mit KI hin, warum, und wie kommen wir dahin?

!!! info "Strategie vs. Aktionismus"
    „Wir setzen jetzt überall KI ein" ist **kein** Ziel, sondern Aktionismus. Eine Strategie verbindet KI mit den **Geschäftszielen**: Welche Ziele unterstützt KI? Welche Use Cases zahlen darauf ein? Ohne diese Verbindung verpuffen Investitionen. Strategie ist die Klammer um alles, was du in diesem Kurs gelernt hast.

---

## 39.2 Bausteine einer KI-Strategie

```mermaid
flowchart TD
    A([Geschäftsziele]) --> B([KI-Vision & Leitplanken])
    B --> C([priorisierte Use Cases])
    C --> D([Roadmap])
    D --> E([Ressourcen: Daten, Skills, Budget])
    E --> F([Governance & Ethik])
```

| Baustein | Frage |
|---|---|
| **Geschäftsziele** | Worauf zahlt KI ein? |
| **Vision & Leitplanken** | Wofür nutzen wir KI – und wofür nicht? |
| **Use Cases** | Welche konkreten Anwendungen (Kap. 4)? |
| **Roadmap** | In welcher Reihenfolge, bis wann? |
| **Ressourcen** | Daten, Kompetenzen, Budget, Werkzeuge |
| **Governance** | Regeln, Verantwortung, Ethik (Block 4) |

!!! info "Vertiefung: Vision und Handlungsfelder"
    Am Anfang steht die **Vision** – ein kurzer, prägnanter Satz, der das Zielbild beschreibt: *„Wir nutzen KI, um unsere Mitarbeitenden von Routinearbeit zu entlasten und schneller auf Kunden zu reagieren."* Eine gute Vision ist konkret genug, um zu leiten, und offen genug, um viele Use Cases zu tragen. Aus ihr leiten sich **Handlungsfelder** ab – thematische Bündel, in denen KI wirken soll, z. B. „Kundenservice", „interne Dokumente", „Produktion" (Kapitel 24). Handlungsfelder sind gröber als einzelne Use Cases: Sie ordnen viele mögliche Anwendungen und verhindern, dass man sich in Einzelideen verzettelt. Erst innerhalb der Handlungsfelder werden konkrete Use Cases gesucht und priorisiert.

---

## 39.3 Use Cases priorisieren und als Roadmap ordnen

Nicht alles auf einmal. Die **Nutzen-Machbarkeit-Matrix** (Kap. 4) hilft, die Reihenfolge zu bestimmen:

| | Geringer Aufwand | Hoher Aufwand |
|---|---|---|
| **Hoher Nutzen** | ✅ zuerst (Quick Wins) | strategische Leuchttürme (planen) |
| **Geringer Nutzen** | nebenbei | vermeiden |

Daraus wird eine **Roadmap** in Wellen:

```mermaid
flowchart LR
    A([Welle 1: Quick Wins z.B. Copilot im Office]) --> B([Welle 2: Prozess-Use-Cases])
    B --> C([Welle 3: strategische / eigene Lösungen])
```

!!! tip "Copilot ist der ideale Start"
    Für die meisten Unternehmen ist die **erste Welle** die breite Einführung von **Copilot** in Office-Aufgaben: hoher Nutzen, geringer Aufwand, keine eigene Infrastruktur (Kap. 7). Das schafft schnelle Erfolge, Akzeptanz und Kompetenz – die Basis für ambitioniertere Wellen.

---

## 39.4 Governance, Kompetenz, Kultur

Eine Strategie ist mehr als eine Use-Case-Liste. Drei „weiche", aber entscheidende Elemente:

| Element | Warum entscheidend |
|---|---|
| **Governance** | Regeln für Datenschutz, Ethik, erlaubte Tools (Block 4, Kap. 11) |
| **Kompetenzaufbau** | ohne Skills keine Nutzung – Schulung, Prompt-Kompetenz (Kap. 40) |
| **Kultur** | Offenheit, Ausprobieren dürfen, Change (Kap. 37) |

!!! warning "Der häufigste Strategiefehler"
    Viele Strategien listen **Technologien und Use Cases**, vergessen aber **Menschen und Regeln**. Dann steht die Technik bereit, aber niemand kann oder darf sie richtig nutzen. Eine gute KI-Strategie plant **Kompetenzaufbau und Governance von Anfang an** mit ein.

---

## 39.5 Eine Strategie-Skizze mit Copilot

**Beispiel-Prompt zum Ausprobieren:**

```text
Ich erstelle eine erste KI-Strategie für ein mittelständisches Unternehmen in
der Branche [Branche]. Hilf mir mit: (1) 3 möglichen strategischen Zielen,
(2) 5 priorisierten Use Cases mit Einordnung nach Nutzen/Aufwand,
(3) einer groben Roadmap in 3 Wellen und (4) den wichtigsten Governance-Punkten.
```

!!! tip "Skizze, nicht Endprodukt"
    Copilot liefert eine schnelle, strukturierte **erste Skizze** – hervorragend als Diskussionsgrundlage. Die echte Strategie entsteht dann im **Dialog mit Führung, Fachbereichen und Betroffenen**, angepasst an eure reale Situation und Datenlage.

---

## 39.6 Make-or-Buy: selbst bauen, kaufen oder anpassen

Für jeden Use Case stellt sich die Frage: **selbst entwickeln (Make)** oder **fertige Lösung nutzen (Buy)**? Zwischen beiden liegt ein Mittelweg – eine Standardlösung **anpassen** (z. B. Copilot mit eigenen Dokumenten anreichern).

| Option | Wann sinnvoll | Beispiel |
|---|---|---|
| **Buy** (kaufen/nutzen) | Standardaufgabe, kein Alleinstellungsmerkmal | Copilot für Office-Arbeit (Kap. 7) |
| **Adapt** (anpassen) | Standard reicht fast, etwas Kontext fehlt | Copilot mit firmeneigenem Wissen |
| **Make** (selbst bauen) | Kernkompetenz, einzigartige Daten, echter Vorteil | eigenes Modell auf Spezialdaten (Kap. 12) |

Faustregel: **Kaufen, was andere auch haben; selbst bauen, was einen Vorteil schafft.** Für den Alltag der meisten Unternehmen ist „Buy/Adapt" der richtige Start – eigene Entwicklung lohnt nur dort, wo sie einen echten **Burggraben** (Kapitel 38) begründet und die Daten- und Kompetenzbasis stimmt (Kapitel 7 – KI-Readiness).

!!! example "Copilot bei der Make-or-Buy-Abwägung"
    Prompt:
    ```text
    Erfinde ein mittelständisches Logistikunternehmen mit drei geplanten
    KI-Use-Cases. Ordne jeden Use Case in Make, Buy oder Adapt ein und begründe
    die Entscheidung in je einem Satz.
    ```
    Beispiel-Antwort (gekürzt):
    ```text
    1) Rechnungen automatisch auslesen -> Buy: Standardproblem, viele fertige
       Werkzeuge vorhanden.
    2) Copilot mit eigenen Prozesshandbüchern nutzen -> Adapt: Standard plus
       firmeneigener Kontext.
    3) Tourenoptimierung auf eigenen Fahrdaten -> Make: einzigartige Daten,
       echter Wettbewerbsvorteil.
    ```

!!! warning "Make ist teurer als es aussieht"
    Ein häufiger Fehler ist, den Aufwand einer Eigenentwicklung zu unterschätzen. „Make" bedeutet nicht nur einmaliges Bauen, sondern **dauerhaften Betrieb**: Daten pflegen, Modelle überwachen, aktualisieren, absichern (Kapitel 35). Ohne diese Ausdauer wird aus dem stolzen Eigenbau schnell ein ungepflegtes Risiko.

---

## Zusammenfassung

- Eine **KI-Strategie** verbindet KI mit **Geschäftszielen** – gegen Aktionismus und Insellösungen.
- Bausteine: **Ziele, Vision/Leitplanken, priorisierte Use Cases, Roadmap, Ressourcen, Governance**.
- Aus der **Vision** leiten sich **Handlungsfelder** ab, in denen konkrete Use Cases gesucht und priorisiert werden.
- Use Cases nach **Nutzen/Aufwand** priorisieren und in **Wellen** ordnen – Copilot-Einführung ist der ideale Start.
- **Make-or-Buy**: kaufen, was andere auch haben; selbst bauen nur, wo es einen echten Vorteil schafft.
- **Governance, Kompetenzaufbau und Kultur** von Anfang an mitplanen – der häufigste Strategiefehler ist, sie zu vergessen.
- **Copilot** liefert eine gute Strategie-**Skizze**; die Ausarbeitung geschieht im Dialog.

---

## Kurzübungen

{{ task(file="tasks/k39_01.yaml") }}

{{ task(file="tasks/k39_02.yaml") }}

{{ task(file="tasks/k39_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k39.yaml") }}
