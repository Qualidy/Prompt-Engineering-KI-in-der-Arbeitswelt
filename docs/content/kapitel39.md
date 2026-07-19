# Kapitel 39 – KI-Strategie und strategisches KI-Management

{{ progress(39) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was eine **KI-Strategie** ist und warum sie nötig ist
- Wie man von der **Vision** zum **Portfolio** von Use Cases kommt
- Was **KI-Governance** bedeutet
- Wie du strategische Überlegungen mit Copilot strukturierst
</div>

---

## 39.1 Warum eine KI-Strategie?

Ohne Strategie entstehen viele **Einzelprojekte ohne roten Faden** – teuer und wirkungslos. Eine **KI-Strategie** richtet den KI-Einsatz an den **Unternehmenszielen** aus.

```mermaid
flowchart LR
    A([Unternehmensziele]) --> B([KI-Vision])
    B --> C([Use-Case-Portfolio])
    C --> D([Umsetzung & Priorisierung])
    D --> E([Governance & Steuerung])
```

---

## 39.2 Von der Vision zum Portfolio

1. **Vision:** Wo wollen wir mit KI hin? (z. B. „datengetriebene Entscheidungen in allen Bereichen")
2. **Handlungsfelder:** Wo lohnt sich KI am meisten?
3. **Use-Case-Portfolio:** konkrete Vorhaben, priorisiert nach Nutzen/Aufwand (Kapitel 4)
4. **Roadmap:** Reihenfolge und Meilensteine

---

## 39.3 KI-Governance

**Governance** sind die **Spielregeln** für KI im Unternehmen:

| Bereich | Frage |
|---|---|
| Verantwortlichkeiten | Wer entscheidet über KI-Einsatz? |
| Richtlinien | Was ist erlaubt (Ethik, Datenschutz, Recht)? |
| Qualität | Wie werden Modelle geprüft und überwacht? |
| Kompetenzen | Wie bauen wir Wissen auf (Prompting!)? |

!!! info "Strategie ohne Umsetzung ist wertlos"
    Eine gute Strategie verbindet **Ambition** mit **realistischer Umsetzung**: klein anfangen, Erfolge zeigen, skalieren.

---

## 39.4 Strategie mit Copilot strukturieren

**Copilot-Prompt zum Ausprobieren:**

```text
Hilf mir, eine einfache KI-Strategie für ein mittelständisches Unternehmen zu
strukturieren: Vision, 3 Handlungsfelder, je 2 Use Cases und die wichtigsten
Governance-Regeln. Stelle es übersichtlich dar.
```

!!! warning "Kontext schlägt Schablone"
    Copilot liefert eine gute **Struktur**, aber die strategischen Entscheidungen hängen von **eurem** Kontext ab. Nutze die Ausgabe als Gerüst, nicht als fertige Strategie.

---

## Kurzübungen

{{ task(file="tasks/k39_01.yaml") }}

{{ task(file="tasks/k39_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k39.yaml") }}
