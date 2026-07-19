# Kapitel 30 – Low-Code-Programmierung und Citizen Development

{{ progress(30) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **Low-Code / No-Code** bedeutet und wer damit arbeitet
- Das Konzept des **Citizen Developers** (Fachanwender ohne Programmierausbildung)
- Wie KI und Low-Code zusammenwirken – bis hin zu **eigenen Copilot-Agenten**
- Ein Überblick über die **Microsoft Power Platform** und **Copilot Studio**
- Welche **Chancen und Risiken (Governance)** damit verbunden sind
</div>

---

## 30.1 Was ist Low-Code / No-Code?

**Low-Code**- und **No-Code**-Plattformen erlauben es, Anwendungen und Automatisierungen **überwiegend visuell** zu erstellen – per Baukasten, statt Zeile für Zeile zu programmieren.

| Begriff | Bedeutung |
|---|---|
| **No-Code** | ganz ohne Programmierung, rein visuell |
| **Low-Code** | wenig Code, meist visuell + optionale Anpassungen |
| **Pro-Code** | klassische Programmierung |

!!! info "Warum das wichtig ist"
    Klassische Softwareentwicklung ist knapp und teuer – IT-Abteilungen kommen mit Anfragen nicht hinterher. Low-Code verschiebt einfache Automatisierungen zu den **Fachbereichen**, die ihre Probleme am besten kennen. Zusammen mit KI (die z. B. aus einer Beschreibung eine App-Idee erzeugt) senkt das die Hürde noch weiter.

---

## 30.2 Der Citizen Developer

Ein **Citizen Developer** ist ein **Fachanwender ohne Programmierausbildung**, der mit Low-Code-Werkzeugen eigene Lösungen baut – z. B. eine Sachbearbeiterin, die einen Genehmigungs-Workflow automatisiert.

```mermaid
flowchart LR
    A([Fachbereich kennt das Problem]) --> B([baut Lösung per Low-Code])
    B --> C([schnelle Automatisierung ohne IT-Stau])
    C --> D([IT sorgt für Rahmen & Sicherheit])
```

!!! example "Typisches Beispiel"
    Statt monatelang auf eine IT-Lösung zu warten, baut die Einkaufsabteilung selbst ein kleines Genehmigungsformular: Antrag ausfüllen → automatische Weiterleitung an die Führungskraft → bei Freigabe Eintrag in eine Liste + Benachrichtigung. Früher ein IT-Projekt, heute eine Nachmittagsaufgabe – mit den richtigen Werkzeugen und **Leitplanken**.

---

## 30.3 Die Microsoft Power Platform

Microsofts Low-Code-Baukasten, eng mit Copilot verzahnt:

| Werkzeug | Wofür |
|---|---|
| **Power Apps** | eigene Apps ohne (viel) Code bauen |
| **Power Automate** | Abläufe automatisieren (Workflows) |
| **Power BI** | Daten auswerten und visualisieren |
| **Copilot Studio** | eigene KI-Assistenten/Chatbots bauen |

### Copilot Studio: eigene KI-Assistenten

Mit **Copilot Studio** kann man – weitgehend ohne Programmierung – **eigene Copilot-Agenten** erstellen: z. B. einen Assistenten, der Fragen zum internen Urlaubsprozess beantwortet, indem er auf die Personalrichtlinien zugreift (RAG, Kap. 5). Man definiert Rolle, Wissensquellen und erlaubte Aktionen – der Bogen zu den KI-Agenten aus Kapitel 5.

---

## 30.4 KI + Low-Code = starke Kombination

KI verstärkt Low-Code auf zwei Ebenen:

1. **KI beim Bauen:** Man beschreibt in Worten, was man will, und die Plattform erzeugt einen ersten Entwurf der App/des Workflows.
2. **KI in der Lösung:** Die gebaute Anwendung nutzt selbst KI (z. B. ein Chatbot, eine automatische Klassifikation von Anfragen).

**Beispiel-Prompt (Konzept mit Copilot vorbereiten):**

```text
Ich möchte einen einfachen Genehmigungsprozess für Urlaubsanträge
automatisieren. Beschreibe Schritt für Schritt, wie ich das mit Power Automate
umsetzen könnte, welche Auslöser und Aktionen ich brauche und worauf ich beim
Datenschutz achten muss.
```

---

## 30.5 Chancen und Risiken (Governance)

| Chance | Risiko |
|---|---|
| schnelle Lösungen aus dem Fachbereich | Wildwuchs unkontrollierter Apps |
| Entlastung der IT | Sicherheits-/Datenschutzlücken |
| mehr Innovation an der Basis | „Schatten-IT" ohne Wartung |
| KI senkt Einstiegshürde weiter | schlecht gebaute, fehleranfällige Lösungen |

!!! warning "Ohne Governance wird Low-Code zum Risiko"
    Wenn jeder unkontrolliert Apps baut, entstehen Sicherheitslücken, doppelte Lösungen und „Schatten-IT", die niemand wartet. Erfolgreiche Unternehmen geben Citizen Developers **klare Leitplanken**: Welche Daten dürfen genutzt werden? Wer prüft und betreibt die Lösung? Das ist Teil der **Data Governance** (Kap. 11) und des verantwortungsvollen KI-Einsatzes (Block 4).

---

## Zusammenfassung

- **Low-Code/No-Code** erlaubt Anwendungen per Baukasten – **Citizen Developers** lösen eigene Probleme.
- Die **Power Platform** (Power Apps, Automate, BI) und **Copilot Studio** sind Microsofts Werkzeuge dafür.
- KI wirkt doppelt: sie hilft **beim Bauen** und steckt **in der Lösung** (z. B. eigene Copilot-Agenten).
- Ohne **Governance** droht Wildwuchs und Schatten-IT – Leitplanken sind Pflicht.

---

## Kurzübungen

{{ task(file="tasks/k30_01.yaml") }}

{{ task(file="tasks/k30_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k30.yaml") }}
