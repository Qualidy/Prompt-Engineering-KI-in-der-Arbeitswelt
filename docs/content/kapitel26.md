# Kapitel 26 – Vorausschauende Wartung (Predictive Maintenance)

{{ progress(26) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **Predictive Maintenance (vorausschauende Wartung)** ist
- Der Unterschied zu **reaktiver** und **präventiver** Wartung
- Wie die **Vorhersage von Ausfällen** technisch grob funktioniert
- Die zwei Wege **Anomalieerkennung** und **Restlebensdauer-Schätzung (RUL)**
- Wie man den **wirtschaftlichen Nutzen** (Business Case) durchrechnet
- Wie **Copilot** bei Wartungsdoku, Analyse und Kommunikation hilft
</div>

---

## 26.1 Drei Wartungsstrategien

Wartung lässt sich auf drei Arten organisieren – vorausschauende Wartung ist die modernste:

| Strategie | Prinzip | Problem |
|---|---|---|
| **Reaktiv** | reparieren, wenn kaputt | teurer Stillstand, Folgeschäden |
| **Präventiv** | nach festem Plan (z. B. alle 6 Monate) | wartet zu früh (Verschwendung) oder zu spät |
| **Vorausschauend** | wartet **genau dann**, wenn Daten es nahelegen | braucht Daten & Modelle |

```mermaid
flowchart LR
    A([Reaktiv: nach Ausfall]) --> B([hoher Stillstand])
    C([Präventiv: fester Plan]) --> D([oft unnötig oder zu spät])
    E([Vorausschauend: datenbasiert]) --> F([Wartung zur richtigen Zeit])
```

!!! info "Warum vorausschauend gewinnt"
    Präventive Wartung nach starrem Kalender tauscht Teile oft aus, die noch funktionieren (Verschwendung) – oder zu spät (Ausfall). **Predictive Maintenance** nutzt den **tatsächlichen Zustand** der Maschine und wartet **im optimalen Moment**: spät genug, um die Lebensdauer auszunutzen, früh genug, um den Ausfall zu verhindern.

---

## 26.2 Wie die Vorhersage funktioniert

Sensoren messen laufend den Zustand (Vibration, Temperatur, Geräusch, Stromaufnahme). Ein Modell hat aus **historischen Daten** gelernt, welche Muster einem Ausfall **vorausgehen**.

```mermaid
flowchart LR
    A([Sensordaten laufend]) --> B([Modell erkennt Verschleißmuster])
    B --> C([Restlebensdauer / Ausfallrisiko schätzen])
    C --> D([Wartung rechtzeitig einplanen])
```

!!! example "Das Prinzip anschaulich"
    Ein Lager, das bald ausfällt, vibriert oft schon Wochen vorher anders – zu leicht, als dass ein Mensch es bemerkt. Das Modell hat aus vielen früheren Ausfällen gelernt, dieses **Frühwarnmuster** zu erkennen, und meldet: „Lager an Maschine 3 wird in ca. 12 Tagen kritisch." Die Instandhaltung plant die Reparatur in die nächste ohnehin geplante Pause.

---

## 26.3 Zwei Wege der Vorhersage

In der Praxis gibt es zwei grundverschiedene Herangehensweisen – sie unterscheiden sich vor allem darin, **wie viele Ausfalldaten** man hat:

| Ansatz | Grundidee | Wann sinnvoll |
|---|---|---|
| **Anomalieerkennung** | lernt den „Normalzustand" und schlägt bei Abweichung Alarm | wenige/keine echten Ausfalldaten |
| **Restlebensdauer (RUL)** | schätzt konkret, wie lange das Teil noch hält | viele dokumentierte Ausfälle vorhanden |

Die **Anomalieerkennung** ist eng mit dem **unüberwachten Lernen** verwandt (Kapitel 12): Das Modell braucht keine markierten Ausfälle, sondern lernt nur, wie „gesund" aussieht, und meldet Auffälligkeiten. Die **Restlebensdauer-Schätzung (Remaining Useful Life)** ist dagegen **überwachtes Lernen**: Sie braucht viele Beispiele, bei denen bekannt ist, wie lange es von einem Zustand bis zum Ausfall dauerte.

!!! info "Vertiefung: Warum echte Ausfalldaten so wertvoll sind"
    Für eine gute Restlebensdauer-Schätzung braucht das Modell viele Beispiele **echter Ausfälle** – und die sind paradox: Je besser ein Betrieb gewartet ist, desto seltener fällt etwas aus, desto weniger Lerndaten gibt es. Deshalb startet man oft mit **Anomalieerkennung** (die ohne Ausfalldaten auskommt) und wechselt erst später, wenn genug Fälle gesammelt sind, zur präziseren RUL-Schätzung. Das erklärt auch, warum Hersteller Ausfalldaten über viele Anlagen hinweg bündeln.

---

## 26.4 Der wirtschaftliche Nutzen

Predictive Maintenance ist ein Paradebeispiel für einen rechenbaren **Business Case**:

| Faktor | Wirkung |
|---|---|
| Weniger ungeplante Stillstände | höhere Verfügbarkeit |
| Weniger Folgeschäden | geringere Reparaturkosten |
| Bessere Ersatzteilplanung | weniger Lagerkosten, keine Hektik |
| Längere Maschinenlebensdauer | Investitionen später nötig |

!!! example "Business Case durchgerechnet"
    Eine Anlage hat bisher pro Jahr **6 ungeplante Ausfälle**. Predictive Maintenance verhindert davon geschätzt **4** (die anderen 2 sind zu spontan). Kosten pro ungeplantem Ausfall:

    | Position | Betrag pro Ausfall |
    |---|---|
    | Stillstand (8 h × 5.000 €/h) | 40.000 € |
    | Folgeschäden/Reparatur | 15.000 € |
    | Eilbestellung Ersatzteil | 5.000 € |
    | **Summe je Ausfall** | **60.000 €** |

    **Vermiedene Kosten:** 4 × 60.000 € = **240.000 €/Jahr**.

    Dem gegenüber stehen die **jährlichen Kosten** der Lösung: Sensorik (Abschreibung) 20.000 € + Softwarelizenz 30.000 € + Betreuung 25.000 € = **75.000 €**.

    **Netto-Nutzen:** 240.000 € − 75.000 € = **165.000 €/Jahr**. Selbst wenn man vorsichtig nur 2 statt 4 verhinderte Ausfälle ansetzt (120.000 €), bleibt der Business Case klar positiv. Genau so baut man ihn auf – die Methodik gilt für viele KI-Projekte (Kapitel 4, 38).

---

## 26.5 Voraussetzungen und Grenzen

!!! warning "Kein Selbstläufer"
    - Man braucht **genügend historische Daten** – idealerweise auch echte Ausfalldaten (die selten und wertvoll sind).
    - **Sensorik** muss vorhanden oder nachrüstbar sein.
    - Für **seltene** Ausfälle ist es schwer, verlässlich zu lernen (wenig Beispiele).
    - Vorhersagen sind **Wahrscheinlichkeiten**, keine Gewissheiten – Fehlalarme und verpasste Fälle bleiben möglich.

---

## 26.6 Wo Copilot unterstützt

Die Vorhersage selbst leistet ein Spezialsystem. **Copilot** hilft rundherum – bei Doku, Auswertung und Kommunikation:

| Aufgabe | Beispiel-Prompt |
|---|---|
| Wartungsberichte | „Fasse diese Wartungshistorie zu den häufigsten Ausfallursachen zusammen." |
| Business Case | „Hilf mir, den Nutzen von Predictive Maintenance für Maschine X zu berechnen." |
| Kommunikation | „Formuliere eine verständliche Info an die Produktion zur geplanten Wartung." |
| Analyse | „Welche Muster zeigt diese Ausfallstatistik (Excel)?" |

**Beispiel-Prompt zum Ausprobieren:**

```text
Erkläre mir den Unterschied zwischen reaktiver, präventiver und vorausschauender
Wartung an einem Beispiel aus einem produzierenden Betrieb. Erstelle dann eine
einfache Beispielrechnung, die den möglichen Nutzen vorausschauender Wartung zeigt.
```

---

## Zusammenfassung

- Drei Strategien: **reaktiv, präventiv, vorausschauend** – Predictive Maintenance wartet **datenbasiert** im optimalen Moment.
- Modelle erkennen aus **Sensordaten** frühe **Verschleißmuster** und schätzen das Ausfallrisiko.
- Zwei Wege: **Anomalieerkennung** (ohne Ausfalldaten) und **Restlebensdauer-Schätzung** (mit vielen Ausfalldaten).
- Der Nutzen (weniger Stillstand/Folgeschäden) ist gut als **Business Case** rechenbar – oft mit sechsstelligem Netto-Nutzen.
- Voraussetzungen: genug **Daten und Sensorik**; Vorhersagen bleiben **Wahrscheinlichkeiten**.
- **Copilot** unterstützt bei Doku, Business Case und Kommunikation – nicht bei der Vorhersage selbst.

---

## Kurzübungen

{{ task(file="tasks/k26_01.yaml") }}

{{ task(file="tasks/k26_02.yaml") }}

{{ task(file="tasks/k26_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k26.yaml") }}
