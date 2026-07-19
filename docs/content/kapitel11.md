# Kapitel 11 – Big Data: Operationalisierung und Prozesse

{{ progress(11) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **Big Data** ausmacht (die „V")
- Wie eine typische **Big-Data-Architektur** aufgebaut ist
- Was **Operationalisierung** bedeutet – vom Datensee zum laufenden Prozess
- Wie Big Data und generative KI (Copilot) zusammenspielen
</div>

---

## 11.1 Was ist Big Data?

**Big Data** bezeichnet Datenmengen, die mit klassischen Mitteln nicht mehr sinnvoll verarbeitet werden können. Charakterisiert durch die **„V"**:

| V | Bedeutung |
|---|---|
| Volume | schiere Menge |
| Velocity | Geschwindigkeit (Echtzeit) |
| Variety | Vielfalt (strukturiert/unstrukturiert) |
| Veracity | Verlässlichkeit/Qualität |
| Value | der geschäftliche Wert |

---

## 11.2 Big-Data-Architektur

```mermaid
flowchart LR
    A([Quellen]) --> B([Ingestion / Erfassung])
    B --> C([Speicherung: Data Lake / Warehouse])
    C --> D([Verarbeitung & Analyse])
    D --> E([Bereitstellung: Dashboards, KI, Apps])
```

| Baustein | Aufgabe |
|---|---|
| Ingestion | Daten aus vielen Quellen einsammeln |
| Data Lake | große Mengen roher Daten speichern |
| Data Warehouse | strukturierte, ausgewertete Daten |
| Verarbeitung | bereinigen, aggregieren, analysieren |
| Bereitstellung | Dashboards, KI-Modelle, Anwendungen |

---

## 11.3 Operationalisierung

**Operationalisierung** heißt: aus einer einmaligen Analyse einen **dauerhaft laufenden Prozess** machen. Daten fließen automatisiert, werden regelmäßig ausgewertet, Ergebnisse landen dort, wo Entscheidungen fallen.

!!! info "Von Projekt zu Betrieb"
    Viele KI-Vorhaben scheitern nicht am Prototyp, sondern am Schritt in den **Regelbetrieb**: Wer pflegt die Daten? Wer überwacht die Qualität? Wer aktualisiert das Modell?

---

## 11.4 Big Data und Copilot

Copilot arbeitet nicht direkt auf riesigen Datenmengen, hilft aber, **Ergebnisse verständlich** zu machen.

**Copilot-Prompt zum Ausprobieren:**

```text
Erkläre die 5 V von Big Data an einem Beispiel aus dem Onlinehandel. Nenne je V
eine konkrete Herausforderung und eine mögliche Lösung.
```

---

## Kurzübungen

{{ task(file="tasks/k11_01.yaml") }}

{{ task(file="tasks/k11_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k11.yaml") }}
