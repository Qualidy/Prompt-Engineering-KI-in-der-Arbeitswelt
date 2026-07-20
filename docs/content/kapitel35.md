# Kapitel 35 – Herausforderungen im KI-Projektmanagement

{{ progress(35) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum KI-Projekte **anders** sind als klassische IT-Projekte
- Die häufigsten **Gründe für das Scheitern** – und wie man sie vermeidet
- Warum KI-Projekte **iterativ und experimentell** sein müssen
- Die Rolle von **interdisziplinären Teams** und klaren **Rollen**
- Wie **Copilot** bei Planung, Doku und Kommunikation im Projekt hilft
</div>

---

## 35.1 Warum KI-Projekte anders sind

Ein klassisches IT-Projekt hat meist ein klar definierbares Ergebnis („die Software macht X"). KI-Projekte sind **unsicherer**: Ob ein Modell die gewünschte Qualität erreicht, weiß man oft erst **nach** dem Ausprobieren mit echten Daten.

| Klassisches IT-Projekt | KI-Projekt |
|---|---|
| Ergebnis vorab spezifizierbar | Ergebnis **datenabhängig**, unsicher |
| linear planbar | **iterativ, experimentell** |
| Erfolg = Spezifikation erfüllt | Erfolg = KPI/Qualität erreicht (statistisch) |
| Daten oft Nebensache | **Daten sind zentral** |

!!! info "Der Kern des Unterschieds"
    Man „bestellt" keine KI-Lösung wie ein fertiges Möbelstück. Man **erforscht**, ob und wie gut sie funktioniert. Das erfordert eine andere Denkweise: **Hypothesen testen** statt „Auftrag abarbeiten". Wer KI-Projekte wie Bauprojekte plant (fixer Umfang, fixer Termin, fixe Qualität), scheitert oft.

---

## 35.2 Warum KI-Projekte scheitern

Studien nennen seit Jahren ähnliche Gründe:

| Grund | Ursache | Gegenmittel |
|---|---|---|
| **Kein klares Problem** | „KI um der KI willen" | vom Problem aus starten (Kap. 4) |
| **Schlechte Daten** | Menge/Qualität unzureichend | Datenrealität früh prüfen (Kap. 9/10) |
| **Kein messbarer Nutzen** | KPI fehlt | KPI vorab definieren |
| **Fehlende Akzeptanz** | Belegschaft zieht nicht mit | Change Management (Kap. 37) |
| **Überzogene Erwartung** | Hype statt Realismus | MVP, klein starten |
| **Keine Operationalisierung** | Pilot geht nie in Betrieb | von Anfang an Betrieb mitdenken (Kap. 11) |

!!! warning "Der 'Pilot-Friedhof'"
    Ein sehr häufiges Muster: Es gibt viele beeindruckende **Piloten**, aber kaum etwas geht in den **Regelbetrieb**. Gründe sind fehlende Integration, unklare Zuständigkeit und mangelnde Akzeptanz. Ein Pilot ist erst dann ein Erfolg, wenn geklärt ist, **wie er skaliert und wer ihn betreibt**.

---

## 35.3 Iterativ und experimentell arbeiten

KI-Projekte folgen einem **Lernzyklus**, nicht einem starren Plan:

```mermaid
flowchart LR
    A([Hypothese]) --> B([kleines Experiment / MVP])
    B --> C([messen an KPI])
    C --> D{lohnt sich?}
    D -->|ja| E([ausbauen])
    D -->|nein| F([anpassen oder stoppen])
    F --> A
```

!!! tip "Das Recht zu scheitern – schnell und günstig"
    Nicht jedes Experiment gelingt – das ist **normal**. Wichtig ist, **schnell und günstig** zu scheitern (kleiner Pilot statt Großprojekt) und daraus zu lernen. Ein früh gestopptes aussichtsloses Projekt ist ein **Erfolg**, kein Versagen.

---

## 35.4 Team und Rollen

KI-Projekte brauchen **verschiedene Kompetenzen** an einem Tisch:

| Rolle | Beitrag |
|---|---|
| **Fachbereich** | kennt Problem, Prozess, Daten (unverzichtbar!) |
| **Daten/IT** | Datenzugang, Technik, Integration |
| **Data Science** (bei Eigenentwicklung) | Modelle, Methodik |
| **Management** | Ziele, Budget, Rückendeckung |
| **Datenschutz/Recht** | Compliance (Block 4) |

!!! info "Der Fachbereich ist der Schlüssel"
    Der häufigste Fehler ist, KI-Projekte rein als „IT-Sache" zu behandeln. Ohne das **Fachwissen** derer, die den Prozess täglich leben, fehlen Problemverständnis, Datenwissen und spätere Akzeptanz. Für Copilot-Einführungen gilt das besonders: Die besten Use Cases kommen aus dem Fachbereich selbst.

---

## 35.5 Copilot als Projekthelfer

Auch die **Projektarbeit selbst** lässt sich mit Copilot beschleunigen:

| Aufgabe | Beispiel-Prompt |
|---|---|
| Projektstruktur | „Erstelle eine grobe Projektstruktur für die Einführung von Copilot im Vertrieb." |
| Risiken | „Nenne die 8 größten Risiken dieses KI-Projekts und je eine Gegenmaßnahme." |
| Statusbericht | „Fasse diese Projektnotizen zu einem knappen Statusbericht zusammen." |
| Kommunikation | „Formuliere eine Info an die Belegschaft zum Start des Pilotprojekts." |

**Beispiel-Prompt zum Ausprobieren:**

```text
Ich plane ein KI-Pilotprojekt zur automatischen Zusammenfassung von
Kundenanfragen. Erstelle einen Plan mit Zielen, einem messbaren KPI, den
größten Risiken und den Rollen, die ich im Team brauche.
```

---

## Zusammenfassung

- KI-Projekte sind **unsicherer** und **datenabhängiger** als klassische IT-Projekte – iterativ statt linear.
- Häufige Scheiterngründe: **kein klares Problem, schlechte Daten, kein KPI, fehlende Akzeptanz, kein Betrieb**.
- Arbeite in **Lernzyklen** (MVP → messen → anpassen); schnelles, günstiges Scheitern ist erlaubt.
- **Interdisziplinäre Teams** mit starkem **Fachbereich** sind entscheidend.
- **Copilot** hilft bei Struktur, Risiken, Statusberichten und Kommunikation.

---

## Kurzübungen

{{ task(file="tasks/k35_01.yaml") }}

{{ task(file="tasks/k35_02.yaml") }}

{{ task(file="tasks/k35_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k35.yaml") }}
