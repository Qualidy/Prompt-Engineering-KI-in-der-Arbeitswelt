# Kapitel 2 – Herkunft und Entwicklung der KI

{{ progress(2) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wo die Idee der Künstlichen Intelligenz **historisch** herkommt
- Die wichtigsten **Meilensteine** von den 1950ern bis zur generativen KI heute
- Was mit den **„KI-Wintern"** gemeint ist und warum es sie gab
- Warum ausgerechnet seit ca. 2012 (und dann 2022) so viel passiert ist
</div>

---

## 2.1 Die Anfänge: eine Idee wird geboren

Die KI ist keine Erfindung der letzten Jahre. Ihre Wurzeln reichen in die **1950er Jahre**:

- **1950** – Alan Turing stellt die Frage „Können Maschinen denken?" und beschreibt den **Turing-Test**.
- **1956** – Auf der **Dartmouth-Konferenz** wird der Begriff *Artificial Intelligence* geprägt. Das gilt als Geburtsstunde der Disziplin.

!!! info "Der Turing-Test"
    Beim Turing-Test kommuniziert ein Mensch per Text mit einem unbekannten Gegenüber. Kann er nicht zuverlässig unterscheiden, ob er mit einem Menschen oder einer Maschine schreibt, hat die Maschine den Test „bestanden". Moderne Chatbots kommen dem in vielen Situationen nahe.

---

## 2.2 Die großen Entwicklungswellen

```mermaid
flowchart LR
    A([1956 Dartmouth]) --> B([1997 Deep Blue])
    B --> C([2012 Deep Learning])
    C --> D([2017 Transformer])
    D --> E([2022 ChatGPT])
    E --> F([2023+ Copilot im Alltag])
```

| Phase | Kennzeichen | Technik |
|---|---|---|
| Symbolische KI (bis 1980er) | Regeln, Logik, „wenn-dann" | Expertensysteme |
| Statistisches Lernen (ab 1990er) | Lernen aus Daten | Machine Learning |
| Deep Learning (ab 2012) | Tiefe neuronale Netze, viele Daten | Bild-/Spracherkennung |
| Generative KI (ab 2022) | Erzeugen von Inhalten | LLMs, Transformer |

---

## 2.3 Die „KI-Winter"

Zweimal (Ende der 1970er und Ende der 1980er) folgte auf große Erwartungen große Ernüchterung: Die Technik konnte die Versprechen nicht halten, Fördergelder wurden gestrichen. Diese Phasen heißen **KI-Winter**.

**Warum kam es dazu?**

- Rechenleistung war zu gering
- Es gab zu wenige digitale Daten
- Die Erwartungen waren unrealistisch hoch (Hype)

!!! warning "Lehre für heute"
    Auch heute gibt es viel Hype um KI. Ein realistischer Blick auf **Nutzen und Grenzen** – statt Über­erwartung – ist ein wichtiger Erfolgsfaktor (siehe Block 5).

---

## 2.4 Warum jetzt alles so schnell geht

Drei Entwicklungen kamen zusammen und beendeten den letzten KI-Winter:

1. **Daten** – Durch Internet, Sensoren und Digitalisierung entstehen riesige Datenmengen.
2. **Rechenleistung** – Grafikkarten (GPUs) und Cloud machen das Training großer Modelle bezahlbar.
3. **Algorithmen** – Die **Transformer-Architektur** (2017) ermöglicht die heutigen Sprachmodelle.

Das Ergebnis: Werkzeuge wie **ChatGPT** und **Microsoft Copilot**, die generative KI für jeden nutzbar machen – ohne Programmierkenntnisse, allein über **Sprache (Prompts)**.

**Copilot-Prompt zum Ausprobieren:**

```text
Erstelle einen kompakten Zeitstrahl der KI-Geschichte mit 6 Meilensteinen.
Formuliere jeden Meilenstein in einem Satz und erkläre, warum er wichtig war.
```

---

## Kurzübungen

{{ task(file="tasks/k02_01.yaml") }}

{{ task(file="tasks/k02_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k02.yaml") }}
