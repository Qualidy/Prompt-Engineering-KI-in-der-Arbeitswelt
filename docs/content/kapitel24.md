# Kapitel 24 – KI in der Produktion

{{ progress(24) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie KI in der **Produktion / Industrie 4.0** eingesetzt wird
- Die Rolle von **Sensoren, IoT und Echtzeitdaten**
- Konkrete Anwendungen: **Qualitätskontrolle, Steuerung, Planung, Wartung**
- Was ein **digitaler Zwilling** ist
- Wo **Copilot** in der Produktionsumgebung sinnvoll unterstützt – und wo nicht
</div>

---

## 24.1 KI und Industrie 4.0

**Industrie 4.0** steht für die Vernetzung von Maschinen, Produkten und Systemen über das Internet. KI ist ihr „Gehirn": Sie wertet die anfallenden Datenmengen aus und trifft oder unterstützt Entscheidungen – oft in **Echtzeit**.

```mermaid
flowchart LR
    A([Sensoren an Maschinen]) --> B([Datenerfassung / IoT])
    B --> C([KI-Analyse in Echtzeit])
    C --> D([Entscheidung / Steuerung])
    D --> E([Aktion an der Maschine])
    E --> A
```

Der Kreislauf ist entscheidend: Maschinen erzeugen laufend Daten, KI wertet sie aus, und das Ergebnis wirkt sofort auf die Produktion zurück.

---

## 24.2 Sensoren, IoT und Echtzeitdaten

Grundlage jeder Produktions-KI sind **Daten aus der Anlage**: Temperatur, Vibration, Druck, Stückzahlen, Bildaufnahmen. Diese liefern **Sensoren**, vernetzt über das **Internet of Things (IoT)**.

!!! info "Warum Echtzeit den Unterschied macht"
    In der Verwaltung darf eine Analyse Stunden dauern. In der Produktion zählt oft die **Millisekunde**: Erkennt die KI einen Fehler erst nach 1.000 produzierten Teilen, ist der Ausschuss teuer. Deshalb laufen viele Produktions-KIs **direkt an der Maschine** (Edge/On-Device, Kap. 5), nicht in einer fernen Cloud.

---

## 24.3 Konkrete Anwendungen

| Anwendung | Was KI tut | Nutzen |
|---|---|---|
| **Optische Qualitätskontrolle** | Kamera + KI erkennt Defekte | weniger Ausschuss, weniger Reklamationen |
| **Prozesssteuerung** | passt Parameter automatisch an | gleichbleibende Qualität |
| **Produktionsplanung** | optimiert Reihenfolge/Auslastung | kürzere Durchlaufzeiten |
| **Vorausschauende Wartung** | sagt Ausfälle voraus | weniger Stillstand (Kap. 26) |
| **Materialfluss/Logistik** | steuert Transporte im Werk | weniger Wartezeit |

!!! example "Optische Qualitätskontrolle in der Praxis"
    Eine Kamera fotografiert jedes Teil am Band; ein Bilderkennungsmodell (Computer Vision, Kap. 1) vergleicht es mit „gut"-Beispielen und sortiert fehlerhafte Teile in Millisekunden aus. Das ist schneller, gleichmäßiger und ermüdungsfrei im Vergleich zur Sichtprüfung durch Menschen – die dafür schwierige Grenzfälle beurteilen.

---

## 24.4 Der digitale Zwilling

Ein **digitaler Zwilling** ist ein virtuelles Abbild einer realen Maschine oder Anlage, gespeist mit deren Echtzeitdaten. Man kann daran **testen und simulieren**, ohne die echte Produktion zu stören.

!!! example "Nutzen"
    „Was passiert, wenn wir die Taktrate um 10 % erhöhen?" – statt es riskant an der echten Anlage auszuprobieren, simuliert man es am digitalen Zwilling. KI hilft, aus den Daten realistische Vorhersagen zu treffen und Optimierungen zu finden.

---

## 24.5 Wo Copilot in der Produktion passt – und wo nicht

Wichtig zur Einordnung: **Copilot ist kein Maschinensteuerungs-System.** Die eigentliche Produktions-KI (Bilderkennung, Steuerung, Predictive Maintenance) sind Spezialsysteme. Copilot hilft am **Rand** – bei Wissen, Kommunikation und Auswertung:

| Aufgabe | Beispiel-Prompt |
|---|---|
| Schichtberichte | „Fasse diese Schichtprotokolle zu den wichtigsten Vorfällen zusammen." |
| Störungsanalyse | „Erkläre mögliche Ursachen für Fehlercode X und Prüfschritte." |
| Doku & Anleitungen | „Erstelle eine verständliche Kurzanleitung aus diesem Handbuchauszug." |
| Auswertung | „Welche Auffälligkeiten zeigt diese Ausschuss-Statistik (Excel)?" |

**Beispiel-Prompt zum Ausprobieren (selbsttragend – Copilot erzeugt die Daten zuerst):**

```text
Erfinde die Schichtprotokolle einer Woche mit mehreren wiederkehrenden Störungen.
Fasse danach die häufigsten Störungen zusammen, ordne sie nach Häufigkeit und
schlage vor, welche zuerst untersucht werden sollten.
```

!!! warning "Klare Grenze"
    Sicherheitskritische Steuerungsentscheidungen trifft **kein** Sprachmodell. Copilot unterstützt bei **Information und Kommunikation**, nicht bei der Echtzeit-Maschinensteuerung. Diese Trennung ist für die Anlagensicherheit essenziell.

---

## Zusammenfassung

- In der Produktion ist KI das „Gehirn" von **Industrie 4.0** – oft in **Echtzeit** direkt an der Maschine.
- Grundlage sind **Sensoren/IoT-Daten**; Anwendungen reichen von **Qualitätskontrolle** bis **Planung**.
- Der **digitale Zwilling** erlaubt gefahrloses Simulieren und Optimieren.
- **Copilot** unterstützt am Rand (Berichte, Doku, Auswertung) – **nicht** die sicherheitskritische Steuerung.

---

## Kurzübungen

{{ task(file="tasks/k24_01.yaml") }}

{{ task(file="tasks/k24_02.yaml") }}

{{ task(file="tasks/k24_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k24.yaml") }}
