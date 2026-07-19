# Kapitel 21 – Prozessoptimierung

{{ progress(21) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **Prozessoptimierung** bedeutet und warum sie ein Top-Einsatzfeld für KI ist
- Wie du einen Prozess **analysierst** und **Engpässe** findest
- Welche **Hebel** KI bietet: automatisieren, beschleunigen, Fehler senken
- Was **Process Mining** ist – Prozesse aus Daten sichtbar machen
- Wie du mit **Copilot** Prozesse dokumentierst, analysierst und verbesserst
</div>

---

## 21.1 Was ist Prozessoptimierung?

Ein **Prozess** ist eine wiederkehrende Abfolge von Tätigkeiten mit einem Ergebnis (z. B. „Angebot erstellen", „Rechnung bearbeiten"). **Prozessoptimierung** macht solche Abläufe **schneller, günstiger, fehlerärmer oder angenehmer**.

!!! info "Warum gerade hier KI wirkt"
    Viele Prozesse enthalten **repetitive, textlastige Schritte**: Daten übertragen, Dokumente lesen, Standardmails schreiben, zusammenfassen. Genau das kann KI (und speziell Copilot) übernehmen oder beschleunigen. Prozessoptimierung ist deshalb eines der **wirkungsvollsten und schnellsten** KI-Einsatzfelder – oft ein Quick Win (Kap. 4).

---

## 21.2 Prozesse analysieren und Engpässe finden

Bevor man optimiert, muss man den Prozess **verstehen**. Ein einfaches Vorgehen:

```mermaid
flowchart LR
    A([Prozess aufnehmen]) --> B([Schritte & Zeiten messen]) --> C([Engpässe finden]) --> D([Verbessern]) --> E([Wirkung prüfen])
    E --> A
```

| Frage | Ziel |
|---|---|
| Welche Schritte gibt es? | Überblick schaffen |
| Wo dauert es lange / staut es sich? | **Engpass (Bottleneck)** finden |
| Wo entstehen Fehler / Nacharbeit? | Qualitätsprobleme finden |
| Welche Schritte sind reine Routine? | Automatisierungskandidaten finden |

!!! tip "Am Engpass ansetzen"
    Eine Kette ist nur so schnell wie ihr langsamstes Glied. Es bringt wenig, einen Schritt zu beschleunigen, der gar nicht der Engpass ist. Finde zuerst den **echten Flaschenhals** – oft ist es ein manueller, textlastiger Schritt, den KI entlasten kann.

---

## 21.3 KI-Hebel in Prozessen

| Hebel | Was passiert | Beispiel mit Copilot |
|---|---|---|
| **Automatisieren** | Routineschritt ganz übernehmen | Standardantworten entwerfen |
| **Beschleunigen** | Menschen schneller machen | Zusammenfassungen, Vorlagen |
| **Fehler senken** | Prüfen, Vollständigkeit sichern | „Fehlt in diesem Antrag etwas?" |
| **Wissen bereitstellen** | schneller die richtige Info finden | interne Doku durchsuchen (RAG) |

---

## 21.4 Process Mining: Prozesse aus Daten sichtbar machen

**Process Mining** rekonstruiert den **tatsächlichen** Prozessablauf aus den digitalen Spuren in IT-Systemen (z. B. Zeitstempel im ERP). So sieht man, wie ein Prozess **wirklich** läuft – nicht wie er im Handbuch stehen sollte.

!!! example "Soll vs. Ist"
    Im Handbuch: „Bestellung → Freigabe → Versand." In den echten Daten zeigt Process Mining vielleicht: In 30 % der Fälle geht es „Bestellung → Versand → nachträgliche Freigabe" – ein Kontrollrisiko, das vorher niemand sah. Solche Abweichungen (**Varianten**) sind der Startpunkt für Verbesserungen.

Process Mining ist meist Aufgabe spezialisierter Tools; Copilot hilft bei der **Interpretation** und **Dokumentation** der Ergebnisse.

---

## 21.5 Prozessarbeit mit Copilot

**Prozess dokumentieren:**

```text
Ich beschreibe dir unseren Angebotsprozess in Stichworten: [Stichworte].
Erstelle daraus eine klare, nummerierte Prozessbeschreibung und markiere
Schritte, die reine Routine sind und sich automatisieren ließen.
```

**Engpässe und Ideen finden:**

```text
Hier ist unser Prozess zur Rechnungsbearbeitung: [Beschreibung].
Analysiere ihn: Wo liegen wahrscheinlich Engpässe und Fehlerquellen?
Schlage 5 konkrete Verbesserungen vor und ordne sie nach Aufwand/Nutzen.
```

**Prozess visualisieren:**

```text
Wandle diese Prozessbeschreibung in eine übersichtliche Schritt-für-Schritt-
Liste mit Verantwortlichkeiten (Rolle je Schritt) um.
```

!!! warning "Copilot kennt euren Prozess nicht von allein"
    Copilot kann nur mit den Informationen arbeiten, die du ihm gibst (oder die es via M365-Daten findet). Beschreibe den Prozess **konkret** – je genauer die Eingabe, desto brauchbarer die Analyse. Und: Vorschläge sind Ideen, keine geprüften Maßnahmen. Die fachliche Bewertung bleibt bei dir und den Beteiligten.

---

## Zusammenfassung

- **Prozessoptimierung** macht wiederkehrende Abläufe besser – ein Top-Einsatzfeld für KI/Copilot.
- Erst **analysieren** und **Engpässe** finden, dann gezielt am Flaschenhals ansetzen.
- KI-Hebel: **automatisieren, beschleunigen, Fehler senken, Wissen bereitstellen**.
- **Process Mining** zeigt den **tatsächlichen** Ablauf aus Daten (Soll vs. Ist).
- **Copilot** hilft beim Dokumentieren, Analysieren und Ideenfinden – konkrete Eingaben sind entscheidend.

---

## Kurzübungen

{{ task(file="tasks/k21_01.yaml") }}

{{ task(file="tasks/k21_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k21.yaml") }}
