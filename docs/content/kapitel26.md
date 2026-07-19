# Kapitel 26 – Vorausschauende Wartung (Predictive Maintenance)

{{ progress(26) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **vorausschauende Wartung** ist und warum sie sich lohnt
- Der Unterschied zu **reaktiver** und **präventiver** Wartung
- Welche **Daten** dafür nötig sind
- Ein **Praxisbeispiel** aus dem Anlagenbetrieb
</div>

---

## 26.1 Drei Wartungsstrategien

| Strategie | Prinzip | Nachteil |
|---|---|---|
| **Reaktiv** | reparieren, wenn kaputt | ungeplante Ausfälle |
| **Präventiv** | feste Intervalle | Wartung zu früh/zu spät |
| **Vorausschauend** | warten, wenn Daten es nahelegen | braucht Daten & Modelle |

**Predictive Maintenance** sagt anhand von Sensordaten voraus, **wann** ein Ausfall droht – und ermöglicht Wartung genau zum richtigen Zeitpunkt.

---

## 26.2 Wie funktioniert das?

```mermaid
flowchart LR
    A([Sensordaten: Temperatur, Vibration, ...]) --> B([KI-Modell])
    B --> C([Zustand & Restlebensdauer schätzen])
    C --> D([Wartung rechtzeitig planen])
```

**Benötigte Daten:**

- Sensordaten (Vibration, Temperatur, Druck, Strom …)
- historische **Ausfalldaten** (wann ist was kaputtgegangen?)
- Wartungshistorie

!!! info "Nutzen"
    Weniger ungeplante Stillstände, längere Maschinenlebensdauer, geplante Ersatzteilbeschaffung, niedrigere Kosten.

---

## 26.3 Voraussetzungen und Grenzen

!!! warning "Ohne Ausfalldaten schwierig"
    Um Ausfälle vorherzusagen, braucht das Modell **Beispiele für Ausfälle**. Bei sehr zuverlässigen Maschinen gibt es davon wenige – dann ist die Prognose schwieriger und man arbeitet mit Anomalieerkennung.

---

## 26.4 Praxisbeispiel: Pumpenüberwachung

!!! info "Fallbeispiel"
    Ein Betreiber überwacht Pumpen mit Vibrations- und Temperatursensoren. Ein Modell erkennt frühzeitig ungewöhnliche Muster und meldet drohende Lagerschäden **Tage vorher**.

    **Ergebnis:** planbare Wartung, keine teuren Notabschaltungen.

**Copilot-Prompt zum Ausprobieren:**

```text
Erkläre Predictive Maintenance an einer Pumpe. Welche Sensordaten sind sinnvoll,
welche historischen Daten braucht das Modell und wie unterscheidet sich der Ansatz
von präventiver Wartung?
```

---

## Kurzübungen

{{ task(file="tasks/k26_01.yaml") }}

{{ task(file="tasks/k26_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k26.yaml") }}
