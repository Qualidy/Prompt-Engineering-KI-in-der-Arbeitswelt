# Kapitel 3 – Einsatz von KI in Unternehmen

{{ progress(3) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum Unternehmen KI einsetzen und welchen **Nutzen** sie sich davon versprechen
- In welchen **Einsatzfeldern** entlang der Wertschöpfungskette KI wirkt
- Wie du **Microsoft Copilot** konkret im Arbeitsalltag nutzt
- Welche typischen **Fehlerwartungen** es gibt
</div>

---

## 3.1 Warum Unternehmen KI einsetzen

Unternehmen setzen KI nicht „der Technik wegen" ein, sondern um konkrete Ziele zu erreichen:

| Ziel | Beispiel |
|---|---|
| **Effizienz** steigern | Routineaufgaben automatisieren, schneller arbeiten |
| **Qualität** verbessern | Fehler früher erkennen, gleichbleibende Ergebnisse |
| **Kosten** senken | Weniger Nacharbeit, bessere Ressourcennutzung |
| **Neue Angebote** schaffen | KI-gestützte Produkte und Services |
| **Entscheidungen** stützen | Prognosen und Auswertungen als Grundlage |

---

## 3.2 Einsatzfelder entlang der Wertschöpfungskette

```mermaid
flowchart LR
    A([Einkauf]) --> B([Produktion])
    B --> C([Marketing & Vertrieb])
    C --> D([Kundenservice])
    D --> E([Verwaltung])
```

| Bereich | Typischer KI-Einsatz |
|---|---|
| Einkauf | Bedarfsprognosen, Lieferantenanalyse |
| Produktion | Qualitätsprüfung, vorausschauende Wartung |
| Marketing & Vertrieb | Personalisierung, Textgenerierung, Lead-Scoring |
| Kundenservice | Chatbots, automatische Ticket-Vorschläge |
| Verwaltung | Dokumentenverarbeitung, Zusammenfassungen, Berichte |

Diese Felder vertiefen wir in **Block 3 (Use Cases)**.

---

## 3.3 Copilot im Arbeitsalltag

**Microsoft Copilot** ist in viele Office-Anwendungen integriert und übernimmt Aufgaben, die viel Zeit kosten:

| Anwendung | Was Copilot kann |
|---|---|
| Word | Entwürfe schreiben, Texte umformulieren, zusammenfassen |
| Outlook | E-Mails entwerfen, Threads zusammenfassen |
| Excel | Formeln erklären, Daten analysieren, Trends benennen |
| Teams | Meetings zusammenfassen, To-dos ableiten |
| PowerPoint | Präsentationen aus Text erzeugen |

**Copilot-Prompt zum Ausprobieren:**

```text
Fasse die folgende E-Mail in 3 Stichpunkten zusammen und schlage eine höfliche
Antwort vor, die um einen Termin nächste Woche bittet:
[E-Mail hier einfügen]
```

!!! tip "Grundregel"
    Je klarer dein **Auftrag** (Rolle, Ziel, Format, Kontext), desto besser die Ausgabe. Das lernst du systematisch in **Kapitel 14 – Prompt Engineering**.

---

## 3.4 Realistische Erwartungen

!!! warning "KI ersetzt nicht das Denken"
    Copilot liefert **Entwürfe**, keine geprüften Endergebnisse. Du bleibst verantwortlich für **Fakten, Ton und Freigabe**. KI ist ein **Assistent**, kein Ersatz für Fachwissen.

---

## Kurzübungen

{{ task(file="tasks/k03_01.yaml") }}

{{ task(file="tasks/k03_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k03.yaml") }}
