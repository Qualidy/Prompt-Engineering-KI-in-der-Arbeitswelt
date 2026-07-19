# Kapitel 28 – KI in der Dokumentenverarbeitung

{{ progress(28) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie KI **Dokumente** automatisch verarbeitet
- Die Schritte: **Erfassen (OCR) → Extrahieren → Klassifizieren → Weiterverarbeiten**
- Wie **Copilot** bei Dokumenten im Arbeitsalltag hilft
- Worauf du bei Vertraulichkeit achten musst
</div>

---

## 28.1 Warum Dokumentenverarbeitung?

Unternehmen ertrinken in Dokumenten: Rechnungen, Verträge, Formulare, E-Mails. **Intelligente Dokumentenverarbeitung (IDP)** automatisiert das Auslesen und Einordnen.

```mermaid
flowchart LR
    A([Dokument]) --> B([OCR: Text erkennen])
    B --> C([Daten extrahieren])
    C --> D([Klassifizieren])
    D --> E([ins System / Workflow])
```

| Schritt | Aufgabe |
|---|---|
| OCR | Bild/Scan in Text umwandeln |
| Extraktion | relevante Felder herausziehen (Betrag, Datum …) |
| Klassifikation | Dokumenttyp erkennen (Rechnung, Vertrag …) |
| Weiterverarbeitung | Daten ins Zielsystem/Workflow geben |

---

## 28.2 Copilot für Dokumente

Copilot glänzt bei **textbasierten** Dokumentenaufgaben:

- **Zusammenfassen** langer Dokumente
- **Extrahieren** von Kernpunkten und Fristen
- **Vergleichen** von Versionen
- **Beantworten** von Fragen zu einem Dokument

**Copilot-Prompt zum Ausprobieren:**

```text
Fasse diesen Vertrag in 5 Stichpunkten zusammen, liste alle Fristen und
Kündigungsregelungen auf und markiere mögliche Risiken:
[Vertragstext einfügen]
```

---

## 28.3 Vertraulichkeit und Prüfung

!!! warning "Sensible Dokumente schützen"
    - Prüfe, ob du **vertrauliche/personenbezogene** Dokumente in ein KI-Werkzeug geben darfst (Unternehmensrichtlinie, DSGVO – Kapitel 33).
    - Nutze die im Unternehmen **freigegebene** Copilot-Umgebung.
    - KI-Ergebnisse (z. B. extrahierte Beträge) **immer prüfen**, bevor sie weiterverarbeitet werden.

!!! info "Menschliche Freigabe"
    Bei rechtlich oder finanziell relevanten Dokumenten bleibt eine **menschliche Kontrolle** vor der Verbuchung/Unterzeichnung Pflicht.

---

## Kurzübungen

{{ task(file="tasks/k28_01.yaml") }}

{{ task(file="tasks/k28_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k28.yaml") }}
