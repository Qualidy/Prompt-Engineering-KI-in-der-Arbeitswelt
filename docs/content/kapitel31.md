# Kapitel 31 – Ethik und soziale Verantwortung

{{ progress(31) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum **Ethik** beim KI-Einsatz wichtig ist
- Was **Bias** (Verzerrung) ist und wie er entsteht
- Zentrale Prinzipien **verantwortungsvoller KI**
- Wie du im Alltag mit Copilot verantwortungsbewusst umgehst
</div>

---

## 31.1 Warum KI-Ethik?

KI trifft oder beeinflusst Entscheidungen, die Menschen betreffen – bei Bewerbungen, Krediten, Diagnosen. Fehler oder Verzerrungen können **reale Nachteile** verursachen. Ethik sorgt dafür, dass KI **fair, transparent und im Sinne der Menschen** eingesetzt wird.

---

## 31.2 Bias: Verzerrungen in KI

**Bias** entsteht, wenn Trainingsdaten die Realität einseitig abbilden. Das Modell übernimmt und verstärkt diese Verzerrung.

```mermaid
flowchart LR
    A([verzerrte Trainingsdaten]) --> B([Modell lernt Verzerrung])
    B --> C([unfaire Entscheidungen])
```

!!! warning "Beispiel"
    Wird ein Bewerbungs-Tool überwiegend mit Lebensläufen einer bestimmten Gruppe trainiert, benachteiligt es systematisch andere – ohne böse Absicht, allein durch die Datenlage.

**Bias-Quellen:** einseitige Daten, historische Ungleichheiten, unausgewogene Beispiele, verzerrte Bewertungen.

---

## 31.3 Prinzipien verantwortungsvoller KI

| Prinzip | Bedeutung |
|---|---|
| Fairness | keine systematische Benachteiligung |
| Transparenz | Entscheidungen nachvollziehbar (Kapitel 34) |
| Verantwortlichkeit | ein Mensch bleibt verantwortlich |
| Datenschutz | Schutz personenbezogener Daten (Kapitel 33) |
| Sicherheit | zuverlässig und robust |
| Menschliche Aufsicht | Mensch kann eingreifen/übersteuern |

---

## 31.4 Verantwortungsvoll mit Copilot arbeiten

**Copilot-Prompt zum Ausprobieren:**

```text
Ich setze KI für [Anwendung] ein. Nenne mögliche ethische Risiken (z. B. Bias,
Diskriminierung, fehlende Transparenz) und je Risiko eine konkrete Gegenmaßnahme.
```

!!! info "Faustregeln"
    - KI-Ausgaben **kritisch prüfen**, nicht blind übernehmen.
    - Bei Entscheidungen über Menschen besonders vorsichtig sein.
    - Verantwortung bleibt **immer beim Menschen**.

---

## Kurzübungen

{{ task(file="tasks/k31_01.yaml") }}

{{ task(file="tasks/k31_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k31.yaml") }}
