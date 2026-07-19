# Kapitel 5 – Aktuelle KI-Trends

{{ progress(5) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Die wichtigsten **aktuellen Trends** der KI und was sie praktisch bedeuten
- Was **generative KI**, **KI-Agenten** und **Multimodalität** sind
- Wohin sich Werkzeuge wie **Microsoft Copilot** entwickeln
- Wie du Trends kritisch einordnest, statt jedem Hype zu folgen
</div>

---

## 5.1 Generative KI

**Generative KI** erzeugt neue Inhalte – Text, Bilder, Audio, Code – auf Basis von Eingaben. Sie ist der Trend, der KI 2022/2023 in den Alltag gebracht hat.

- Beispiele: Copilot, ChatGPT, Bildgeneratoren
- Für Unternehmen relevant, weil sie **ohne Programmierung** über Sprache bedienbar ist

---

## 5.2 KI-Agenten

Ein **KI-Agent** löst nicht nur eine einzelne Anfrage, sondern verfolgt ein **Ziel** über mehrere Schritte – er plant, nutzt Werkzeuge und handelt teilweise selbstständig.

```mermaid
flowchart LR
    A([Ziel]) --> B([Plan erstellen])
    B --> C([Schritte ausführen / Tools nutzen])
    C --> D([Ergebnis prüfen])
    D -->|nicht fertig| B
    D -->|fertig| E([Ergebnis])
```

Beispiel: Ein Agent, der eigenständig Termine recherchiert, Vorschläge macht und eine E-Mail entwirft. Microsoft entwickelt Copilot in diese Richtung weiter (**Copilot Agents**).

---

## 5.3 Multimodalität

**Multimodale** KI verarbeitet mehrere Datenarten gleichzeitig – Text, Bild, Ton. Du kannst Copilot z. B. ein Bild zeigen und eine Frage dazu stellen.

| Modalität | Beispiel-Aufgabe |
|---|---|
| Text | Zusammenfassen, übersetzen |
| Bild | Diagramm erklären, Foto beschreiben |
| Audio | Meeting transkribieren |
| Kombination | Aus Skizze + Text einen Entwurf erstellen |

---

## 5.4 Weitere Trends im Blick

- **Kleine, spezialisierte Modelle (SLMs):** effizienter, teils lokal auf dem Gerät
- **KI-Regulierung:** der EU AI Act setzt Leitplanken (siehe Kapitel 32)
- **Individualisierung:** Modelle werden an Unternehmensdaten angepasst

**Copilot-Prompt zum Ausprobieren:**

```text
Nenne die drei wichtigsten KI-Trends für kleine und mittlere Unternehmen in
diesem Jahr. Erkläre je Trend in 2 Sätzen die praktische Bedeutung und nenne
ein konkretes Beispiel.
```

!!! warning "Trend ≠ Pflicht"
    Nicht jeder Trend passt zu jedem Unternehmen. Frage immer: Löst dieser Trend ein **echtes Problem** bei uns?

---

## Kurzübungen

{{ task(file="tasks/k05_01.yaml") }}

{{ task(file="tasks/k05_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k05.yaml") }}
