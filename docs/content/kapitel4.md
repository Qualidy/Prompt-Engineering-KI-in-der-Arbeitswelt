# Kapitel 4 – Entwicklung und Umsetzung von KI-Konzepten

{{ progress(4) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie aus einer **Idee** ein tragfähiger **KI-Use-Case** wird
- Ein bewährtes **Vorgehensmodell** für KI-Projekte
- Wie du Ideen nach **Machbarkeit** und **Wert** priorisierst
- Wie **Copilot** dich beim Konzipieren unterstützt
</div>

---

## 4.1 Von der Idee zum Use Case

Nicht jede Idee ist ein guter KI-Use-Case. Ein tragfähiger Use Case beantwortet klar:

- **Problem:** Welches konkrete Problem lösen wir?
- **Daten:** Welche Daten stehen zur Verfügung – in welcher Qualität?
- **Nutzen:** Was ist der messbare Vorteil (Zeit, Geld, Qualität)?
- **Machbarkeit:** Ist es technisch und organisatorisch umsetzbar?

---

## 4.2 Ein Vorgehensmodell für KI-Projekte

Viele KI-Projekte folgen einem iterativen Ablauf, angelehnt an das bekannte Modell **CRISP-DM**:

```mermaid
flowchart LR
    A([Geschäftsverständnis]) --> B([Datenverständnis])
    B --> C([Datenaufbereitung])
    C --> D([Modellierung])
    D --> E([Evaluation])
    E --> F([Einsatz / Betrieb])
    E -.->|nachschärfen| B
```

| Phase | Leitfrage |
|---|---|
| Geschäftsverständnis | Welches Ziel verfolgen wir? |
| Datenverständnis | Welche Daten haben wir? |
| Datenaufbereitung | Sind die Daten sauber und nutzbar? |
| Modellierung | Welches Verfahren/Werkzeug passt? |
| Evaluation | Erfüllt das Ergebnis die Ziele? |
| Einsatz | Wie bringen wir es in den Betrieb? |

!!! info "Iterativ statt linear"
    KI-Projekte laufen selten geradlinig. Oft muss man zu früheren Phasen zurückkehren – z. B. weil die Datenqualität nicht reicht.

---

## 4.3 Ideen priorisieren: Nutzen vs. Machbarkeit

Nicht alles gleichzeitig umsetzen. Eine einfache **Nutzen-Machbarkeit-Matrix** hilft:

| | Geringer Aufwand | Hoher Aufwand |
|---|---|---|
| **Hoher Nutzen** | ✅ Quick Win – zuerst! | Strategisches Projekt |
| **Geringer Nutzen** | Nice-to-have | ❌ vermeiden |

---

## 4.4 Copilot beim Konzipieren nutzen

Copilot eignet sich hervorragend, um Konzepte zu **strukturieren** und **Lücken** zu finden.

**Copilot-Prompt zum Ausprobieren:**

```text
Ich möchte einen KI-Use-Case für [Prozess] konzipieren. Stelle mir strukturiert
die 6 wichtigsten Fragen, die ich vorher klären muss, und erkläre kurz, warum
jede Frage wichtig ist.
```

!!! tip "Copilot als Sparringspartner"
    Lass dir Konzepte nicht abnehmen, sondern **hinterfragen**: „Welche Risiken übersehe ich?", „Welche Daten brauche ich mindestens?". So nutzt du KI als Denkwerkzeug.

---

## Kurzübungen

{{ task(file="tasks/k04_01.yaml") }}

{{ task(file="tasks/k04_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k04.yaml") }}
