# Kapitel 28 – KI in der Dokumentenverarbeitung

{{ progress(28) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum **Dokumentenverarbeitung** eines der stärksten KI-Einsatzfelder im Büro ist
- Die typische **Verarbeitungskette**: erfassen, extrahieren, klassifizieren, prüfen, weiterleiten
- Was **OCR, Extraktion und Klassifikation** bedeuten
- Wie **Copilot** Dokumente zusammenfasst, durchsucht und Daten herauszieht
- Welche **Fehlerrisiken** bestehen und wie du sie absicherst
</div>

---

## 28.1 Warum Dokumente ein idealer KI-Fall sind

Unternehmen ertrinken in Dokumenten: Rechnungen, Verträge, Berichte, E-Mails, Formulare, Protokolle. Vieles davon ist **unstrukturierter Text** (Kap. 9) – genau das, was moderne Sprach-KI besonders gut verarbeitet.

!!! info "Der Hebel"
    Dokumentenarbeit ist oft **zeitraubend, repetitiv und fehleranfällig**: lesen, verstehen, wichtige Daten heraussuchen, ablegen. Genau diese Kette kann KI stark beschleunigen. Deshalb gehört Dokumentenverarbeitung zu den **schnellsten und lohnendsten** Einsatzfeldern – ein klassischer Quick Win (Kap. 4).

---

## 28.2 Die Verarbeitungskette

```mermaid
flowchart LR
    A([Erfassen: Scan/Datei]) --> B([OCR: Text lesbar machen])
    B --> C([Klassifizieren: welcher Dokumenttyp?])
    C --> D([Extrahieren: relevante Daten])
    D --> E([Prüfen: plausibel/vollständig?])
    E --> F([Weiterleiten/Ablegen])
```

| Schritt | Was passiert | Beispiel |
|---|---|---|
| **Erfassen** | Dokument digitalisieren | Rechnung scannen |
| **OCR** | Bild → maschinenlesbarer Text | gescanntes PDF wird durchsuchbar |
| **Klassifizieren** | Dokumententyp bestimmen | „das ist eine Rechnung" |
| **Extrahieren** | Kernangaben herausziehen | Betrag, Datum, Lieferant |
| **Prüfen** | Plausibilität/Vollständigkeit | „Betrag fehlt?" |
| **Weiterleiten** | ins Zielsystem/an Zuständige | Buchhaltung |

### OCR, Extraktion, Klassifikation kurz erklärt

- **OCR (Texterkennung):** wandelt ein **Bild** von Text (Scan, Foto) in **echten Text** um, mit dem man arbeiten kann.
- **Klassifikation:** ordnet ein Dokument einer **Kategorie** zu (Rechnung, Angebot, Mahnung …).
- **Extraktion:** zieht **gezielt Datenfelder** heraus (Rechnungsnummer, Betrag, Datum).

---

## 28.3 Dokumentenarbeit mit Copilot

**Copilot** ist im Büroalltag extrem stark bei Text-Dokumenten:

| Aufgabe | Beispiel-Prompt |
|---|---|
| Zusammenfassen | „Fasse dieses 12-seitige Dokument in 7 Kernpunkten zusammen." |
| Gezielt fragen | „Was steht in diesem Vertrag zur Kündigungsfrist?" |
| Daten extrahieren | „Zieh aus dieser Rechnung Nummer, Datum, Betrag, Lieferant als Tabelle." |
| Vergleichen | „Was hat sich zwischen diesen zwei Vertragsversionen geändert?" |
| Umformen | „Mach aus diesem Protokoll eine To-do-Liste mit Verantwortlichen." |

**Beispiel-Prompt zum Ausprobieren:**

```text
Analysiere den folgenden Vertragstext. Erstelle eine Tabelle mit:
Vertragspartner, Laufzeit, Kündigungsfrist, monatliche Kosten, besondere
Klauseln. Markiere alle Angaben, die im Text nicht eindeutig zu finden sind.
```

!!! tip "Der 'markiere Unsicheres'-Trick"
    Die Anweisung, **unsichere oder fehlende Angaben ausdrücklich zu markieren**, ist Gold wert: So siehst du sofort, wo du nachprüfen musst, statt einer scheinbar vollständigen Tabelle blind zu vertrauen.

---

## 28.4 Fehlerrisiken und Absicherung

!!! warning "Wo es schiefgehen kann"
    - **Zahlendreher/Extraktionsfehler:** Ein falsch gelesener Betrag in der Buchhaltung ist teuer – kritische Werte gegen das Original prüfen.
    - **Halluzinierte Inhalte:** Bei fehlenden Angaben kann das Modell etwas „Plausibles" erfinden (Kap. 15).
    - **Vertraulichkeit:** Verträge und personenbezogene Dokumente nur in der **freigegebenen** M365-Umgebung verarbeiten (Kap. 33).
    - **Vollautomatik ohne Kontrolle:** Bei rechts-/geldrelevanten Dokumenten sollte ein Mensch prüfen (Human-in-the-Loop).

!!! info "Automatisierung mit Augenmaß"
    Ein bewährtes Muster: KI verarbeitet und schlägt vor, ein Mensch **prüft die kritischen Fälle** (z. B. hohe Beträge, unklare Extraktionen). So bekommt man Tempo **und** Sicherheit. Für große Volumina gibt es spezialisierte Systeme (z. B. Azure AI Document Intelligence); für den Alltag genügt oft Copilot.

---

## Zusammenfassung

- Dokumentenverarbeitung ist ein **Top-Einsatzfeld** – viel unstrukturierter Text, viel Routine.
- Die Kette: **Erfassen → OCR → Klassifizieren → Extrahieren → Prüfen → Weiterleiten**.
- **Copilot** ist stark beim Zusammenfassen, Durchsuchen, Extrahieren und Vergleichen von Dokumenten.
- Absicherung: **kritische Werte prüfen**, Unsicheres markieren lassen, Vertraulichkeit wahren, Human-in-the-Loop.

---

## Kurzübungen

{{ task(file="tasks/k28_01.yaml") }}

{{ task(file="tasks/k28_02.yaml") }}

{{ task(file="tasks/k28_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k28.yaml") }}
