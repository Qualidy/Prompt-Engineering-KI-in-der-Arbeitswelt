# Kapitel 29 – KI für Nachhaltigkeit und Ressourceneffizienz

{{ progress(29) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie KI zu **Nachhaltigkeit** und **Ressourceneffizienz** beitragen kann
- Konkrete Anwendungen: **Energie, Material, Logistik, Kreislaufwirtschaft**
- Das **Spannungsfeld**: KI spart Ressourcen – verbraucht aber selbst welche
- Was der **Rebound-Effekt** ist und warum Effizienz allein nicht reicht
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

Der Kern ist immer derselbe: KI verwandelt **Messdaten in bessere Entscheidungen**. Wo früher grobe Faustregeln oder Durchschnittswerte galten, kann ein Modell den tatsächlichen Bedarf im Einzelfall abschätzen – und genau das ist der Hebel für Ressourceneffizienz.

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

!!! info "Vertiefung: Warum Vorhersage der Schlüssel ist"
    Viele Ressourcen werden verschwendet, weil Menschen **auf Vorrat** handeln: Man heizt lieber zu viel als zu wenig, produziert lieber einen Puffer als eine Fehlmenge, fährt lieber die volle Route als das Risiko einer Lücke. Diese Sicherheitszuschläge kosten Energie und Material. KI reduziert die Unsicherheit durch bessere **Prognosen** (Kap. 26 – Predictive Maintenance, Kap. 21 – Prozessoptimierung). Je genauer man den Bedarf **kennt**, desto kleiner darf der Puffer sein – das ist die eigentliche Quelle der Einsparung.

---

## 29.3 Das Spannungsfeld: KI verbraucht selbst Ressourcen

!!! warning "Ehrliche Bilanz nötig"
    KI ist **kein reiner Umweltretter**. Das **Training** großer Modelle und ihr laufender Betrieb verbrauchen viel **Strom und Wasser** (Kühlung der Rechenzentren) – mehr dazu in Kapitel 36. Eine seriöse Bewertung fragt: Spart der KI-Einsatz **mehr** Ressourcen, als er selbst verbraucht? Nur dann ist er auch ökologisch sinnvoll.

Für **Nutzer:innen von Copilot** ist der eigene Verbrauch pro Anfrage klein, summiert sich aber über Millionen Anfragen. Bewusster Einsatz (keine sinnlosen Massen-Prompts, keine zehn Varianten „zum Spaß") ist Teil verantwortungsvoller Nutzung. Eine faire Bilanz betrachtet immer den **gesamten Lebenszyklus**: Training, Betrieb und die Frage, ob die eingesparte Ressource den Aufwand rechtfertigt.

---

## 29.4 Der Rebound-Effekt: Effizienz allein reicht nicht

Ein häufig übersehener Fallstrick ist der **Rebound-Effekt**: Wenn etwas effizienter (und damit billiger) wird, nutzt man oft **mehr** davon – und ein Teil der Einsparung verpufft.

```mermaid
flowchart LR
    A([KI macht Prozess effizienter]) --> B([Kosten pro Einheit sinken])
    B --> C([Nutzung steigt])
    C --> D([Teil der Einsparung verpufft])
```

Ein klassisches Beispiel außerhalb der KI: Ein sparsameres Auto verbraucht pro Kilometer weniger – aber weil Fahren billiger wird, fährt man mehr. Übertragen auf KI: Wenn das Erstellen von Texten, Bildern oder Auswertungen fast nichts mehr kostet, produziert man plötzlich **viel mehr** davon. Der Nettoeffekt für die Umwelt kann dann sogar negativ sein.

!!! warning "Effizienz ist nicht gleich Nachhaltigkeit"
    Ein verbreitetes Missverständnis lautet: „KI macht alles effizienter, also ist KI automatisch nachhaltig." Das stimmt nicht. Effizienz senkt den Verbrauch **pro Einheit**, sagt aber nichts über die **Gesamtmenge** aus. Nachhaltig wird der Einsatz erst, wenn die Effizienzgewinne nicht vollständig durch Mehrnutzung aufgefressen werden. Deshalb gehört zu jeder KI-Nachhaltigkeitsmaßnahme die Frage: „Was passiert mit der eingesparten Ressource?"

Der **KI-Fußabdruck** eines Unternehmens umfasst also nicht nur den Strom eines einzelnen Modells, sondern auch das durch KI **zusätzlich ausgelöste** Verhalten (mehr Inhalte, mehr Rechenläufe, mehr Geräte). Nachhaltige Governance setzt hier bewusst Grenzen und Prioritäten.

---

## 29.5 KI und ESG-Berichterstattung

Unternehmen müssen zunehmend über **Nachhaltigkeit berichten** – Stichwort **ESG** (Environmental, Social, Governance) und EU-Vorgaben (z. B. CSRD). Das bedeutet viel **Datensammlung und Textarbeit** – ein gutes Feld für Copilot.

| Aufgabe | Wie KI hilft |
|---|---|
| Daten zusammentragen | verstreute Angaben bündeln |
| Kennzahlen erklären | komplexe Werte verständlich aufbereiten |
| Berichte entwerfen | Textbausteine, Struktur, Zusammenfassungen |
| Lücken finden | „Welche Angaben fehlen für Standard X?" |

!!! warning "ESG-Zahlen sind prüfungsrelevant"
    Nachhaltigkeitsangaben werden zunehmend geprüft und dürfen nicht beschönigt werden – schöngefärbte Berichte gelten als **Greenwashing** und sind ein rechtliches wie reputatives Risiko (Kap. 31 – Ethik, Kap. 32 – Recht). Copilot darf hier **formulieren und strukturieren**, aber niemals Zahlen „erfinden" oder glätten. Jede Kennzahl im Bericht muss auf eine belegbare Quelle zurückführbar sein.

---

## 29.6 Nachhaltigkeitsarbeit mit Copilot

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

Damit du das gefahrlos üben kannst, lässt du Copilot die Datenbasis **selbst erfinden** – so brauchst du keine echten Betriebsdaten hochzuladen:

!!! example "Ausgearbeiteter Copilot-Dialog"
    **Prompt:**
    ```text
    Erfinde eine fiktive Tabelle mit dem monatlichen Stromverbrauch (kWh) eines
    kleinen Produktionsbetriebs über 12 Monate, inklusive eines auffälligen
    Ausreißers. Analysiere sie danach: Nenne den Trend, den Ausreißer und drei
    konkrete Einsparansätze. Sag ehrlich, welche Annahmen du triffst.
    ```
    **Beispiel-Antwort von Copilot (gekürzt):**
    ```text
    Fiktive Daten (kWh): Jan 12.400 · Feb 11.900 · Mär 12.100 · Apr 10.800
    · Mai 10.200 · Jun 9.800 · Jul 15.600 · Aug 9.500 · Sep 10.100 ...

    Trend: Verbrauch sinkt im Frühjahr/Sommer – plausibel durch weniger Heizung.
    Ausreißer: Juli (15.600 kWh) liegt ~55 % über dem Nachbarmonat.
    Ansätze:
    1. Ursache des Juli-Peaks prüfen (Klimatisierung? Sonderschicht?).
    2. Grundlast nachts messen – Standby-Verbräuche senken.
    3. Lastspitzen glätten, um teure Spitzentarife zu vermeiden.

    Annahme: Werte sind erfunden; realer Nutzen entsteht erst mit echten Zählern.
    ```

Der letzte Satz ist entscheidend: Copilot liefert eine **plausible Struktur und Denkrichtung**, aber die Zahlen sind fiktiv. Der Wert liegt im **Analyseraster**, das du dann auf echte, geprüfte Daten anwendest.

!!! tip "Von der Idee zur Maßnahme"
    Copilot ist gut darin, aus Daten **Einsparideen** und aus Vorgaben **Berichtsstrukturen** zu erzeugen. Die **Umsetzung und Verifikation** (stimmen die Zahlen? ist die Maßnahme realistisch?) bleibt beim Team. Achte bei Berichtsangaben besonders auf Faktenprüfung – Nachhaltigkeitszahlen sind zunehmend prüfungsrelevant.

---

## Zusammenfassung

- KI findet **Einsparpotenziale** bei Energie, Material, Logistik, Landwirtschaft und im Kreislauf.
- Das Prinzip ist **Präzision**: „genau so viel wie nötig" statt pauschal – gute **Prognosen** verkleinern Sicherheitspuffer.
- **Spannungsfeld:** KI verbraucht selbst Ressourcen (Kap. 36) – der Nettoeffekt muss positiv sein.
- **Rebound-Effekt:** Effizienz allein reicht nicht, wenn die Mehrnutzung die Einsparung auffrisst; der **KI-Fußabdruck** umfasst auch das ausgelöste Verhalten.
- Bei **ESG-Berichten** hilft Copilot beim Bündeln, Erklären und Entwerfen – Zahlen bleiben prüfpflichtig, Greenwashing ist tabu.

---

## Kurzübungen

{{ task(file="tasks/k29_01.yaml") }}

{{ task(file="tasks/k29_02.yaml") }}

{{ task(file="tasks/k29_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k29.yaml") }}
