# Kapitel 10 – Datenaufbereitung

{{ progress(10) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum **Datenaufbereitung** oft 60–80 % der Projektzeit kostet
- Die typischen **Schritte** der Aufbereitung: bereinigen, transformieren, anreichern
- Häufige **Datenprobleme** und wie man sie erkennt
- Was **„Garbage in, garbage out"** praktisch bedeutet
- Wie **Copilot in Excel** bei der Datenaufbereitung hilft – und wo Grenzen sind
</div>

---

## 10.1 Warum Datenaufbereitung so wichtig ist

Rohdaten sind fast nie direkt nutzbar. Sie sind unvollständig, uneinheitlich, fehlerhaft oder doppelt. Bevor KI oder Analysen sinnvolle Ergebnisse liefern, müssen die Daten **aufbereitet** werden.

!!! info "Die 80-Prozent-Regel"
    In vielen Datenprojekten entfallen **60–80 % der Zeit** auf Beschaffung und Aufbereitung – und nur ein kleiner Teil auf die eigentliche „KI". Das ist unspektakulär, aber der Hebel für Qualität. Wer hier schludert, bekommt es später doppelt zurück.

---

## 10.2 Der Grundsatz: Garbage in, garbage out

```mermaid
flowchart LR
    A([schlechte Daten]) --> B([Modell / Analyse]) --> C([schlechte Ergebnisse])
    D([gute Daten]) --> E([Modell / Analyse]) --> F([verlässliche Ergebnisse])
```

Egal wie modern der Algorithmus: Sind die Eingangsdaten fehlerhaft, sind es auch die Ergebnisse. Ein Prognosemodell, das mit falschen Verkaufszahlen gefüttert wird, liefert falsche Prognosen – überzeugend formatiert, aber wertlos. Dasselbe gilt für Copilot: Fasst es ein fehlerhaftes Dokument zusammen, ist die Zusammenfassung ebenfalls fehlerhaft.

---

## 10.3 Die Schritte der Datenaufbereitung

| Schritt | Ziel | Beispiel |
|---|---|---|
| **Bereinigen** | Fehler und Lücken beheben | fehlende Werte, Tippfehler, Ausreißer |
| **Vereinheitlichen** | einheitliches Format | Datum, Einheiten, Schreibweisen |
| **Entdoppeln** | Dubletten entfernen | derselbe Kunde mehrfach |
| **Transformieren** | Form für die Nutzung bringen | Text → Kategorien, Werte skalieren |
| **Anreichern** | zusätzliche Infos ergänzen | Postleitzahl → Region |

### Typische Datenprobleme im Detail

| Problem | Beispiel | Folge, wenn ignoriert |
|---|---|---|
| Fehlende Werte | Feld „Umsatz" ist leer | verzerrte Summen/Durchschnitte |
| Uneinheitliche Formate | „01.02.2026" vs. „2026-02-01" | Fehler beim Sortieren/Rechnen |
| Dubletten | Kunde „Müller GmbH" doppelt | Kunde wird doppelt gezählt |
| Ausreißer | Alter „199" | verfälscht Statistiken |
| Inkonsistenzen | „DE" vs. „Deutschland" | Gruppierung schlägt fehl |

!!! tip "Erst verstehen, dann bereinigen"
    Bevor du Daten „reparierst", frage: **Warum** fehlt der Wert? Ein fehlender Umsatz kann „0 €" bedeuten – oder „nicht erfasst". Das ist ein großer Unterschied. Blindes Auffüllen mit Nullen kann Ergebnisse stärker verfälschen als die Lücke selbst.

---

## 10.4 Datenaufbereitung mit Copilot in Excel

**Copilot in Excel** unterstützt viele Aufbereitungsschritte per Sprachbefehl – ideal für alle, die keine Formel-Profis sind.

| Aufgabe | Beispiel-Prompt |
|---|---|
| Probleme finden | „Prüfe diese Tabelle auf fehlende Werte und Auffälligkeiten." |
| Formate erklären/ändern | „Wandle die Datumsspalte in das Format JJJJ-MM-TT um." |
| Formeln erzeugen | „Erstelle eine Formel, die Dubletten in Spalte A markiert." |
| Analysieren | „Welche Trends und Ausreißer zeigt diese Tabelle?" |

**Beispiel-Prompt zum Ausprobieren:**

```text
Analysiere die markierte Tabelle: Nenne fehlende Werte je Spalte, mögliche
Dubletten und Ausreißer. Schlage für jedes Problem einen konkreten
Bereinigungsschritt vor.
```

!!! warning "Copilot ersetzt keine Prüfung"
    Copilot **schlägt** Bereinigungen vor – die Entscheidung triffst du. Prüfe jeden Vorschlag: Ist ein „Ausreißer" ein Fehler oder ein echter Sonderfall? Werden beim Entdoppeln vielleicht berechtigte Einträge gelöscht? Gerade bei Daten kann eine falsche Automatik still und leise Schaden anrichten.

!!! info "Sensible Daten"
    Lade keine vertraulichen oder personenbezogenen Daten in Werkzeuge, für die es keine Freigabe gibt. Innerhalb der freigegebenen Microsoft-365-Umgebung bewegst du dich im geschützten Rahmen – außerhalb nicht (Kapitel 33).

---

## Zusammenfassung

- Datenaufbereitung ist der **zeitintensivste** und qualitätsentscheidende Teil (60–80 %).
- **„Garbage in, garbage out"**: schlechte Daten → schlechte Ergebnisse, egal wie gut der Algorithmus.
- Kernschritte: **bereinigen, vereinheitlichen, entdoppeln, transformieren, anreichern**.
- **Copilot in Excel** hilft beim Finden und Beheben von Problemen – die fachliche Prüfung bleibt bei dir.

---

## Kurzübungen

{{ task(file="tasks/k10_01.yaml") }}

{{ task(file="tasks/k10_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k10.yaml") }}
