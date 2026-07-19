# Kapitel 10 – Datenaufbereitung

{{ progress(10) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum Rohdaten fast nie direkt nutzbar sind
- Die typischen Schritte der **Datenaufbereitung** (Cleaning, Transformation, Feature Engineering)
- Was eine **Datenpipeline** ist
- Wie **Copilot** in Excel bei der Aufbereitung hilft
</div>

---

## 10.1 Warum aufbereiten?

Rohdaten sind meist unvollständig, uneinheitlich oder fehlerhaft. Die **Datenaufbereitung** macht sie erst analyse- und trainierbar. Faustregel: In vielen Projekten fließen **60–80 %** des Aufwands in diesen Schritt.

---

## 10.2 Die Schritte der Datenaufbereitung

```mermaid
flowchart LR
    A([Rohdaten]) --> B([Bereinigen])
    B --> C([Transformieren])
    C --> D([Anreichern / Feature Engineering])
    D --> E([Analysebereite Daten])
```

| Schritt | Was passiert |
|---|---|
| Bereinigen (Cleaning) | Dubletten entfernen, fehlende Werte behandeln, Fehler korrigieren |
| Transformieren | Formate vereinheitlichen, skalieren, kodieren |
| Anreichern | zusätzliche Merkmale bilden (Feature Engineering) |
| Zusammenführen | Daten aus mehreren Quellen verbinden |

---

## 10.3 Typische Probleme und Lösungen

| Problem | Lösung |
|---|---|
| Fehlende Werte | löschen, ersetzen (Mittelwert), markieren |
| Dubletten | erkennen und zusammenführen |
| Uneinheitliche Formate | Standardisieren (z. B. Datumsformat) |
| Ausreißer | prüfen, ob Fehler oder echte Werte |

!!! info "Feature Engineering"
    Ein **Feature** ist ein Merkmal, das dem Modell hilft. Beispiel: Aus einem Kaufdatum lässt sich das Merkmal „Wochentag" ableiten – das kann für eine Prognose entscheidend sein.

---

## 10.4 Datenaufbereitung mit Copilot in Excel

Copilot kann in **Excel** viele Aufbereitungsschritte erklären und ausführen.

**Copilot-Prompt zum Ausprobieren (in Excel):**

```text
Analysiere diese Tabelle auf Datenqualität: Nenne Spalten mit fehlenden Werten,
mögliche Dubletten und uneinheitliche Formate. Schlage konkrete Schritte zur
Bereinigung vor.
```

!!! warning "Ergebnisse prüfen"
    Copilot macht Vorschläge – die **fachliche Prüfung** bleibt bei dir. Gerade beim Ersetzen fehlender Werte kann eine falsche Methode das Ergebnis verzerren.

---

## Kurzübungen

{{ task(file="tasks/k10_01.yaml") }}

{{ task(file="tasks/k10_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k10.yaml") }}
