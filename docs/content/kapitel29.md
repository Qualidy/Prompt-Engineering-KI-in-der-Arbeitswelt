# Kapitel 29 – KI für Nachhaltigkeit und Ressourceneffizienz

{{ progress(29) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie KI zu **Nachhaltigkeit** und **Ressourceneffizienz** beitragen kann
- Konkrete Anwendungen: **Energie, Material, Logistik, Kreislaufwirtschaft**
- Das **Spannungsfeld**: KI spart Ressourcen – verbraucht aber selbst welche
- Was **ESG-Berichterstattung** ist und wie KI dabei hilft
- Wie **Copilot** bei Analyse und Nachhaltigkeitsdokumentation unterstützt
</div>

---

## 29.1 KI als Werkzeug für Nachhaltigkeit

Nachhaltigkeit heißt, mit **Ressourcen** (Energie, Material, Zeit) sparsam umzugehen. KI ist dafür gut geeignet, weil sie in großen Datenmengen **Einsparpotenziale** findet, die Menschen übersehen, und Prozesse **feiner optimiert**.

```mermaid
flowchart LR
    A([Daten: Energie, Material, Prozesse]) --> B([KI findet Muster & Optima])
    B --> C([Empfehlung/Steuerung])
    C --> D([weniger Verbrauch / weniger Abfall])
```

---

## 29.2 Konkrete Anwendungen

| Bereich | KI-Anwendung | Effekt |
|---|---|---|
| **Energie** | Verbrauch vorhersagen, Anlagen effizient regeln | weniger Strom/Wärme |
| **Material** | Ausschuss senken, Zuschnitt optimieren | weniger Abfall |
| **Logistik** | Routen und Auslastung optimieren | weniger Leerfahrten/CO₂ |
| **Landwirtschaft** | Wasser/Dünger präzise dosieren | Ressourcen schonen |
| **Kreislaufwirtschaft** | Materialien sortieren/wiederverwerten | Recyclingquote steigt |
| **Gebäude** | Heizung/Kühlung bedarfsgerecht (Kap. 27) | Energie sparen |

!!! example "Präzision spart Ressourcen"
    Statt ein ganzes Feld gleichmäßig zu düngen, ermittelt KI aus Sensordaten, **welche Teilfläche wie viel** braucht (Precision Farming). Ergebnis: gleicher Ertrag mit weniger Dünger und Wasser. Dasselbe Prinzip – „genau so viel wie nötig" – wirkt auch bei Energie und Material.

---

## 29.3 Das Spannungsfeld: KI verbraucht selbst Ressourcen

!!! warning "Ehrliche Bilanz nötig"
    KI ist **kein reiner Umweltretter**. Das **Training** großer Modelle und ihr laufender Betrieb verbrauchen viel **Strom und Wasser** (Kühlung der Rechenzentren) – mehr dazu in Kapitel 36. Eine seriöse Bewertung fragt: Spart der KI-Einsatz **mehr** Ressourcen, als er selbst verbraucht? Nur dann ist er auch ökologisch sinnvoll.

Für **Nutzer:innen von Copilot** ist der eigene Verbrauch pro Anfrage klein, summiert sich aber über Millionen Anfragen. Bewusster Einsatz (keine sinnlosen Massen-Prompts) ist Teil verantwortungsvoller Nutzung.

---

## 29.4 KI und ESG-Berichterstattung

Unternehmen müssen zunehmend über **Nachhaltigkeit berichten** – Stichwort **ESG** (Environmental, Social, Governance) und EU-Vorgaben (z. B. CSRD). Das bedeutet viel **Datensammlung und Textarbeit** – ein gutes Feld für Copilot.

| Aufgabe | Wie KI hilft |
|---|---|
| Daten zusammentragen | verstreute Angaben bündeln |
| Kennzahlen erklären | komplexe Werte verständlich aufbereiten |
| Berichte entwerfen | Textbausteine, Struktur, Zusammenfassungen |
| Lücken finden | „Welche Angaben fehlen für Standard X?" |

---

## 29.5 Nachhaltigkeitsarbeit mit Copilot

**Beispiel-Prompts:**

```text
Analysiere diese monatlichen Stromverbrauchsdaten (Excel): Nenne Trends,
Auffälligkeiten und drei konkrete Ansatzpunkte, um Energie einzusparen.
```

```text
Erstelle das Gliederungsgerüst für einen Nachhaltigkeitsbericht eines
mittelständischen Produktionsbetriebs entlang der ESG-Dimensionen. Markiere
je Abschnitt, welche Daten ich dafür beschaffen muss.
```

!!! tip "Von der Idee zur Maßnahme"
    Copilot ist gut darin, aus Daten **Einsparideen** und aus Vorgaben **Berichtsstrukturen** zu erzeugen. Die **Umsetzung und Verifikation** (stimmen die Zahlen? ist die Maßnahme realistisch?) bleibt beim Team. Achte bei Berichtsangaben besonders auf Faktenprüfung – Nachhaltigkeitszahlen sind zunehmend prüfungsrelevant.

---

## Zusammenfassung

- KI findet **Einsparpotenziale** bei Energie, Material, Logistik, Landwirtschaft und im Kreislauf.
- Das Prinzip ist **Präzision**: „genau so viel wie nötig" statt pauschal.
- **Spannungsfeld:** KI verbraucht selbst Ressourcen (Kap. 36) – der Nettoeffekt muss positiv sein.
- Bei **ESG-Berichten** hilft Copilot beim Bündeln, Erklären und Entwerfen – Zahlen bleiben prüfpflichtig.

---

## Kurzübungen

{{ task(file="tasks/k29_01.yaml") }}

{{ task(file="tasks/k29_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k29.yaml") }}
