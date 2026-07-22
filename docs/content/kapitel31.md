# Kapitel 31 – Ethik und soziale Verantwortung

{{ progress(31) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum **Ethik** bei KI kein „Beiwerk", sondern geschäftskritisch ist
- Was **Bias (Verzerrung)** ist, wie er entsteht und welche Folgen er hat
- Zentrale ethische Prinzipien: **Fairness, Transparenz, Verantwortung, Nicht-Schaden**
- Die Auswirkungen von KI auf **Arbeit und Gesellschaft**
- Wie du im Alltag – auch mit **Copilot** – verantwortungsvoll handelst
</div>

---

## 31.1 Warum KI-Ethik geschäftskritisch ist

KI-Systeme treffen oder beeinflussen Entscheidungen, die **Menschen betreffen**: wer einen Kredit bekommt, wer zum Vorstellungsgespräch eingeladen wird, welche Diagnose vorgeschlagen wird. Fehler oder Verzerrungen haben hier **reale Folgen**.

!!! info "Nicht nur 'nice to have'"
    Ethik ist bei KI nicht bloß eine moralische Frage, sondern **geschäftskritisch**: Diskriminierende oder intransparente KI führt zu **Rechtsstreit, Bußgeldern (EU AI Act, Kap. 32), Reputationsschäden** und Vertrauensverlust. Verantwortungsvolle KI ist damit auch ein **wirtschaftliches** Gebot.

---

## 31.2 Bias: die verzerrte KI

**Bias** (Verzerrung) bedeutet, dass ein KI-System bestimmte Gruppen systematisch **benachteiligt** oder ein schiefes Weltbild widerspiegelt. Die Hauptursache: **verzerrte Trainingsdaten**.

```mermaid
flowchart LR
    A([verzerrte Trainingsdaten]) --> B([Modell lernt die Verzerrung])
    B --> C([verzerrte Entscheidungen])
    C --> D([Benachteiligung realer Menschen])
```

!!! example "Der klassische Fall"
    Ein Unternehmen trainiert eine Bewerbungs-KI mit den Einstellungsdaten der letzten 10 Jahre. Wurden damals überwiegend Männer eingestellt, „lernt" die KI, männliche Bewerber zu bevorzugen – nicht aus Absicht, sondern weil sie das **Muster der Vergangenheit** reproduziert. Genau das ist mehreren realen Unternehmen passiert. Die KI ist dabei nur ein **Spiegel** der Daten.

!!! warning "Auch Copilot ist nicht neutral"
    Sprachmodelle lernen aus riesigen Textmengen aus dem Internet – inklusive der darin enthaltenen **Vorurteile und Einseitigkeiten**. Antworten können daher stereotype oder einseitige Sichtweisen enthalten. Man muss aktiv gegensteuern (z. B. um ausgewogene Darstellung bitten) und Ergebnisse **kritisch prüfen**.

---

## 31.3 Ethische Grundprinzipien

| Prinzip | Bedeutung | Praktische Frage |
|---|---|---|
| **Fairness** | keine Diskriminierung | Werden Gruppen benachteiligt? |
| **Transparenz** | nachvollziehbar, offengelegt | Weiß der Mensch, dass/wie KI beteiligt ist? |
| **Verantwortung** | jemand haftet | Wer verantwortet die Entscheidung? |
| **Nicht-Schaden** | kein Schaden für Menschen | Welche negativen Folgen sind möglich? |
| **Selbstbestimmung** | Mensch behält Kontrolle | Kann der Mensch widersprechen/eingreifen? |

Diese Prinzipien finden sich auch in offiziellen Leitlinien (z. B. der EU) und im **EU AI Act** wieder (Kap. 32).

---

## 31.4 KI, Arbeit und Gesellschaft

KI verändert die Arbeitswelt – das wirft ehrliche Fragen auf:

| Chance | Sorge |
|---|---|
| Entlastung von Routine | Wegfall von Tätigkeiten |
| neue Berufsbilder (z. B. Prompt-Kompetenz) | Qualifikationsdruck |
| höhere Produktivität | Überwachung/Kontrolle am Arbeitsplatz |
| bessere Entscheidungen | Verantwortungsdiffusion („die KI war's") |

!!! info "Realistische Einordnung"
    Die Erfahrung zeigt: KI ersetzt meist **Aufgaben**, nicht ganze **Menschen**. Berufe verändern sich – repetitive Anteile fallen weg, dafür kommen Steuerung, Prüfung und Kommunikation hinzu. Deshalb ist **Weiterbildung** (wie dieser Kurs) die beste Antwort auf die Sorgen. Verantwortungsvolle Unternehmen nehmen die Belegschaft aktiv mit (Change Management, Kap. 37).

---

## 31.5 Verantwortungsvoll handeln mit Copilot

Konkrete Leitplanken für den Alltag:

- **Prüfen statt vertrauen:** Ergebnisse auf Fakten, Fairness und Ton kontrollieren.
- **Transparenz:** offenlegen, wenn Inhalte KI-gestützt entstanden sind (wo relevant).
- **Keine heiklen Entscheidungen delegieren:** über Menschen (Personal, Bewertung) entscheiden Menschen.
- **Bias aktiv entgegenwirken:** ausgewogene Perspektiven anfordern.

**Copilot-Prompt zum Ausprobieren (selbsttragend – Copilot erzeugt den Text zuerst):**

```text
Schreibe einen kurzen Text über eine Berufsgruppe, der unbewusst einige Stereotype
enthält. Prüfe ihn danach auf mögliche Stereotype oder einseitige Formulierungen und
schlage neutralere, ausgewogene Alternativen vor.
```

!!! tip "Ethik ist eine Haltung, kein Häkchen"
    Verantwortungsvolle KI-Nutzung entsteht nicht durch ein einmaliges Regelwerk, sondern durch eine **wache Grundhaltung** bei jeder Anwendung: „Wen betrifft das? Kann das ungerecht wirken? Muss ich das offenlegen?"

---

## Zusammenfassung

- KI-Ethik ist **geschäftskritisch** – wegen Recht, Bußgeldern, Reputation und Vertrauen.
- **Bias** entsteht aus verzerrten Daten; KI ist ein **Spiegel** – auch Copilot ist nicht neutral.
- Leitprinzipien: **Fairness, Transparenz, Verantwortung, Nicht-Schaden, Selbstbestimmung**.
- KI ersetzt meist **Aufgaben**, nicht Menschen – **Weiterbildung** und Mitnahme der Belegschaft sind zentral.
- Im Alltag: prüfen, offenlegen, heikle Entscheidungen beim Menschen lassen, Bias entgegenwirken.

---

## Kurzübungen

{{ task(file="tasks/k31_01.yaml") }}

{{ task(file="tasks/k31_02.yaml") }}

{{ task(file="tasks/k31_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k31.yaml") }}
