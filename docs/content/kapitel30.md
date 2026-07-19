# Kapitel 30 – Low-Code-Programmierung und Citizen Development

{{ progress(30) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **Low-Code/No-Code** bedeutet
- Wer ein **Citizen Developer** ist
- Wie **KI** und Low-Code zusammenspielen (z. B. Microsoft Power Platform)
- Chancen und Risiken für Unternehmen
</div>

---

## 30.1 Was ist Low-Code/No-Code?

**Low-Code**- und **No-Code**-Plattformen ermöglichen es, Anwendungen weitgehend **ohne** klassisches Programmieren zu erstellen – per Baukasten, Drag-and-drop und Vorlagen.

| Begriff | Bedeutung |
|---|---|
| No-Code | ganz ohne Code, rein visuell |
| Low-Code | überwiegend visuell, wenig Code für Sonderfälle |

---

## 30.2 Citizen Development

Ein **Citizen Developer** ist eine Fachkraft **ohne** Informatikausbildung, die mit Low-Code eigene Lösungen baut – z. B. eine App zur Urlaubsverwaltung oder einen automatisierten Genehmigungs-Workflow.

```mermaid
flowchart LR
    A([Fachkraft mit Problem]) --> B([Low-Code-Plattform])
    B --> C([eigene App/Automatisierung])
    C --> D([Problem im Team gelöst])
```

!!! info "Warum das boomt"
    Fachbereiche kennen ihre Probleme am besten. Low-Code erlaubt es ihnen, kleine Lösungen **selbst** zu bauen – schnell und ohne lange IT-Warteschlange.

---

## 30.3 KI + Low-Code: Microsoft Power Platform

Microsofts **Power Platform** (Power Apps, Power Automate, Copilot Studio) verbindet Low-Code mit KI:

- **Power Apps:** Apps per Baukasten
- **Power Automate:** Abläufe automatisieren
- **Copilot Studio:** eigene Chatbots/Agenten ohne tiefes Coding
- **Copilot-Beschreibung:** App/Flow per **natürlicher Sprache** erzeugen lassen

**Copilot-Prompt-Idee (in Power Platform):**

```text
Erstelle eine App, mit der Mitarbeitende Urlaubsanträge einreichen und
Vorgesetzte sie genehmigen können. Speichere die Anträge in einer Liste.
```

---

## 30.4 Chancen und Risiken

| Chancen | Risiken |
|---|---|
| schnelle Lösungen | Wildwuchs („Schatten-IT") |
| Entlastung der IT | Sicherheits-/Datenschutzlücken |
| Innovation im Fachbereich | fehlende Wartung/Dokumentation |

!!! warning "Governance nötig"
    Citizen Development braucht **Leitplanken**: Wer darf was bauen? Wo liegen Daten? Wer betreut die Lösung? Ohne Regeln entstehen Sicherheits- und Wartungsprobleme.

---

## Kurzübungen

{{ task(file="tasks/k30_01.yaml") }}

{{ task(file="tasks/k30_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k30.yaml") }}
