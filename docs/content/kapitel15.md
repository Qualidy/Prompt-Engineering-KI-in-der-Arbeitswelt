# Kapitel 15 – Large Language Models und ihre Programmierung

{{ progress(15) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was ein **Large Language Model (LLM)** ist
- Das Grundprinzip: **Vorhersage des nächsten Wortes**
- Wichtige Begriffe: **Kontextfenster**, **Temperatur**, **System-Prompt**
- Wie man LLMs „programmiert" – über Anweisungen statt klassischem Code
</div>

---

## 15.1 Was ist ein LLM?

Ein **Large Language Model** ist ein sehr großes, mit riesigen Textmengen trainiertes KI-Modell. Es kann Sprache verstehen und erzeugen. **Copilot**, ChatGPT und Gemini basieren auf LLMs.

„Large" bezieht sich auf die **Anzahl der Parameter** (interne Stellschrauben) – oft viele Milliarden.

---

## 15.2 Das Grundprinzip: nächstes Wort vorhersagen

Ein LLM macht im Kern **eine** Sache extrem gut: Es sagt das **wahrscheinlich nächste Wort** (Token) voraus – und wiederholt das Wort für Wort.

```mermaid
flowchart LR
    A(["Der Kunde bestellt eine ..."]) --> B([LLM])
    B --> C(["... Rechnung? Pizza? Software?"])
    C --> D([wählt wahrscheinlichstes Wort])
```

!!! info "Erstaunlich mächtig"
    Aus diesem einfachen Prinzip entstehen zusammenhängende Texte, Übersetzungen und Code – weil das Modell dabei enorm viel Sprach- und Weltwissen aus dem Training nutzt.

---

## 15.3 Wichtige Begriffe

| Begriff | Bedeutung | Praxis |
|---|---|---|
| **Kontextfenster** | wie viel Text das Modell „gleichzeitig sehen" kann | zu lange Eingaben werden abgeschnitten |
| **Temperatur** | wie „kreativ"/zufällig die Ausgabe ist | niedrig = sachlich, hoch = kreativer |
| **System-Prompt** | Grundanweisung, die das Verhalten festlegt | z. B. „Antworte immer förmlich auf Deutsch" |
| **Token** | Text-Baustein (siehe Kapitel 13) | Abrechnung/Limits erfolgen in Tokens |

---

## 15.4 Wie man LLMs „programmiert"

Der große Unterschied zur klassischen Software: Du steuerst ein LLM überwiegend durch **Sprache**, nicht durch Code.

| Weg | Beschreibung | Für wen |
|---|---|---|
| **Prompting** | Anweisungen in natürlicher Sprache | alle Anwender (Copilot) |
| **System-Prompt** | dauerhafte Verhaltensregeln | Power-User, Admins |
| **API** | LLM aus eigenen Programmen aufrufen | Entwickler |
| **Fine-Tuning** | Modell mit eigenen Daten nachtrainieren | Spezialfälle |

**Copilot-Prompt zum Ausprobieren:**

```text
Erkläre mir den Unterschied zwischen einem normalen Prompt und einem
System-Prompt an einem Beispiel. Wann sollte ich welchen einsetzen?
```

!!! warning "Grenzen kennen"
    Ein LLM „weiß" nichts sicher – es erzeugt **wahrscheinliche** Texte. Es kann überzeugend klingende, aber falsche Antworten geben (**Halluzinationen**). Prüfen bleibt Pflicht.

---

## Kurzübungen

{{ task(file="tasks/k15_01.yaml") }}

{{ task(file="tasks/k15_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k15.yaml") }}
