# Kapitel 32 – Rechtliche Aspekte der KI

{{ progress(32) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Welche **Rechtsgebiete** beim KI-Einsatz berührt werden
- Was der **EU AI Act** ist und wie sein **risikobasierter Ansatz** funktioniert
- Fragen zu **Urheberrecht, Haftung und Kennzeichnung**
- Warum **„der Mensch bleibt verantwortlich"** rechtlich zentral ist
- Wie du im Alltag mit **Copilot** rechtssicher(er) arbeitest
</div>

---

## 32.1 Ein Überblick: berührte Rechtsgebiete

KI ist kein rechtsfreier Raum – im Gegenteil, sie berührt viele Bereiche gleichzeitig:

| Rechtsgebiet | Beispiel-Frage |
|---|---|
| **KI-Regulierung** (EU AI Act) | Welche Pflichten hat unser KI-System? |
| **Datenschutz** (DSGVO) | Dürfen wir diese personenbezogenen Daten nutzen? (Kap. 33) |
| **Urheberrecht** | Wem gehören Eingaben und Ergebnisse? |
| **Haftung** | Wer haftet für einen KI-Fehler? |
| **Arbeitsrecht** | Mitbestimmung bei KI am Arbeitsplatz? |
| **Wettbewerbs-/Vertragsrecht** | Zusicherungen, Werbung mit KI |

!!! warning "Dieser Kurs ersetzt keine Rechtsberatung"
    Die folgenden Punkte schaffen **Orientierung** und Problembewusstsein – im konkreten Fall ist **juristischer Rat** einzuholen. Ziel ist, dass du **weißt, wann** eine rechtliche Prüfung nötig ist.

---

## 32.2 Der EU AI Act

Der **EU AI Act** ist das weltweit erste umfassende KI-Gesetz. Sein Kern ist ein **risikobasierter Ansatz**: Je höher das Risiko einer KI-Anwendung, desto strenger die Pflichten.

```mermaid
flowchart TD
    A([Inakzeptables Risiko: verboten]) 
    B([Hohes Risiko: strenge Auflagen])
    C([Begrenztes Risiko: Transparenzpflichten])
    D([Minimales Risiko: kaum Auflagen])
```

| Risikostufe | Beispiele | Folge |
|---|---|---|
| **Inakzeptabel** | Social Scoring, manipulative Systeme | **verboten** |
| **Hoch** | KI in Personalauswahl, Kreditvergabe, Medizin | strenge Pflichten (Doku, Aufsicht, Qualität) |
| **Begrenzt** | Chatbots, generierte Inhalte | **Transparenz** (Kennzeichnung) |
| **Minimal** | Spamfilter, Spiele | kaum Auflagen |

!!! info "Was das praktisch heißt"
    Nutzt du Copilot zum Texten von E-Mails, bist du im **minimalen/begrenzten** Bereich. Setzt ein Unternehmen KI für **Einstellungsentscheidungen** ein, ist das **Hochrisiko** – mit umfangreichen Pflichten. Die zentrale Frage lautet also immer: **Wofür** wird die KI genau eingesetzt?

---

## 32.3 Urheberrecht, Haftung, Kennzeichnung

### Urheberrecht

- **Eingaben:** Fremde geschützte Werke nicht ungefragt hochladen/verarbeiten.
- **Ausgaben:** Ob und wem KI-generierte Inhalte urheberrechtlich „gehören", ist teils **ungeklärt** und je nach Land unterschiedlich. Für kommerzielle Nutzung genau prüfen.

### Haftung

!!! warning "Die KI haftet nicht"
    Ein KI-System ist keine juristische Person – es kann nicht haften. Verantwortlich bleibt immer der **Mensch bzw. das Unternehmen**, das die KI einsetzt. „Die KI hat den Fehler gemacht" ist **keine** Entschuldigung vor Gericht oder Kunden. Deshalb ist die **Prüfung** von KI-Ergebnissen nicht nur Sorgfalt, sondern rechtliche Notwendigkeit.

### Kennzeichnung

Der EU AI Act verlangt zunehmend, dass **KI-generierte oder -manipulierte Inhalte** (Texte, Bilder, „Deepfakes") als solche **gekennzeichnet** werden (Bezug zu Kap. 19).

---

## 32.4 „Human in the Loop" als rechtliches Prinzip

Weil der Mensch verantwortlich bleibt, ist die menschliche Kontrolle (**Human in the Loop**) bei bedeutsamen Entscheidungen nicht nur gute Praxis, sondern rechtlich geboten. Die DSGVO gibt Menschen z. B. ein Recht, **nicht ausschließlich** einer automatisierten Entscheidung unterworfen zu werden (Kap. 33).

---

## 32.5 Rechtssicherer arbeiten mit Copilot

Praktische Leitplanken:

- **Freigegebene Umgebung nutzen:** Microsoft 365 Copilot verarbeitet Daten im geschützten Unternehmensrahmen (Kap. 33).
- **Keine fremden geschützten Werke** ungefragt einspeisen.
- **Ergebnisse prüfen und verantworten** – besonders bei rechtlich/wirtschaftlich Relevantem.
- **Kennzeichnen**, wo KI-Inhalte offengelegt werden müssen.
- **Interne Richtlinie** beachten (Was ist erlaubt? Welche Tools?).

**Copilot-Prompt zum Ausprobieren:**

```text
Erkläre den risikobasierten Ansatz des EU AI Act in einfachen Worten und ordne
drei Beispiele (Spamfilter, Kundenservice-Chatbot, KI in der Personalauswahl)
den passenden Risikostufen zu. Nenne je eine Pflicht, die daraus folgt.
```

---

## Zusammenfassung

- KI berührt viele Rechtsgebiete: **EU AI Act, DSGVO, Urheberrecht, Haftung, Arbeitsrecht**.
- Der **EU AI Act** arbeitet **risikobasiert** – vom Verbot bis zu minimalen Auflagen; entscheidend ist der **Einsatzzweck**.
- **Die KI haftet nie** – Verantwortung bleibt beim Menschen/Unternehmen; Ergebnisse prüfen ist Pflicht.
- **Kennzeichnung** von KI-Inhalten und **Human in the Loop** werden rechtlich zunehmend verlangt.
- Im Zweifel: **Rechtsberatung** einholen und interne Richtlinien beachten.

---

## Kurzübungen

{{ task(file="tasks/k32_01.yaml") }}

{{ task(file="tasks/k32_02.yaml") }}

{{ task(file="tasks/k32_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k32.yaml") }}
