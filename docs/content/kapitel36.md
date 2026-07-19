# Kapitel 36 – Energie- und Ressourcenverbrauch von KI

{{ progress(36) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Warum KI **Energie, Wasser und Rohstoffe** verbraucht – und wo genau
- Der Unterschied im Verbrauch zwischen **Training** und **Nutzung (Inferenz)**
- Größenordnungen: Was kostet eine KI-Anfrage die Umwelt (grob)?
- Wie Anbieter und Nutzer den **Fußabdruck senken** können
- Wie du als **Copilot-Nutzer:in** bewusst und effizient umgehst
</div>

---

## 36.1 KI ist nicht „immateriell"

KI wirkt körperlos – doch dahinter stehen **riesige Rechenzentren** mit hohem Verbrauch an:

| Ressource | Wofür |
|---|---|
| **Strom** | Rechenleistung (v. a. GPUs) für Training und Nutzung |
| **Wasser** | Kühlung der Rechenzentren |
| **Rohstoffe** | Hardware (Chips, seltene Metalle) |

!!! info "Die unsichtbaren Kosten"
    Jede Copilot-Antwort läuft auf physischer Hardware, die Strom zieht und gekühlt werden muss. Einzeln ist der Verbrauch klein, in der **Masse** aber erheblich. Nachhaltige KI-Nutzung (Kap. 29) setzt voraus, diese Seite ehrlich mitzudenken – sonst „spart" man an einer Stelle und verbraucht an anderer mehr.

---

## 36.2 Training vs. Nutzung

Der Verbrauch verteilt sich auf zwei sehr unterschiedliche Phasen:

```mermaid
flowchart LR
    A([Training: einmalig, sehr energieintensiv]) --> B([fertiges Modell])
    B --> C([Nutzung/Inferenz: pro Anfrage klein])
    C --> D([summiert über Milliarden Anfragen: sehr groß])
```

| Phase | Verbrauch | Charakter |
|---|---|---|
| **Training** | sehr hoch, aber **einmalig** | wie ein großer Bau |
| **Nutzung (Inferenz)** | pro Anfrage klein | aber **milliardenfach** täglich |

!!! example "Warum beides zählt"
    Das **Training** eines sehr großen Modells kann so viel Energie verbrauchen wie hunderte Haushalte in einem Jahr – aber es passiert nur einmal. Die **Nutzung** kostet pro Prompt wenig, doch bei **weltweit Milliarden** Anfragen täglich summiert sich das zu einem enormen Dauerverbrauch. Beide Phasen sind daher relevant.

---

## 36.3 Größenordnungen einordnen

Genaue Zahlen schwanken je nach Modell und Rechenzentrum stark und werden selten offengelegt. Wichtiger als exakte Werte ist das **Größengefühl**:

- Eine KI-Textanfrage verbraucht deutlich **mehr** Energie als eine klassische Websuche.
- Bild- und Videogenerierung ist **energieintensiver** als reine Textausgabe.
- Der Wasserverbrauch für Kühlung ist real und in wasserarmen Regionen ein Thema.

!!! warning "Vorsicht bei kursierenden Zahlen"
    Im Netz kursieren viele konkrete Verbrauchszahlen („X Liter Wasser pro Anfrage") – sie sind oft **Schätzungen** mit großen Unsicherheiten oder veraltet. Nutze sie zur **Sensibilisierung**, nicht als exakte Fakten, und prüfe die Quelle (Anwendung von Kap. 15: nicht jeder plausiblen Zahl trauen).

---

## 36.4 Den Fußabdruck senken

**Was Anbieter tun (können):**

| Hebel | Wirkung |
|---|---|
| Erneuerbare Energie für Rechenzentren | geringerer CO₂-Fußabdruck |
| Effizientere Hardware und Kühlung | weniger Strom/Wasser |
| **Kleinere, spezialisierte Modelle** (SLMs) | weniger Verbrauch pro Aufgabe (Kap. 5) |
| Standortwahl (Klima, grüner Strom) | weniger Kühlbedarf |

**Was Nutzer:innen tun können:**

- **Bewusst prompten:** klare Prompts statt endloser Trial-and-Error-Serien.
- **Das richtige Werkzeug** für die Aufgabe – nicht für jede Kleinigkeit ein großes Modell.
- **Massenhafte, sinnlose Generierung vermeiden** (z. B. „mach mir mal 500 Varianten zum Spaß").

!!! tip "Effizientes Prompten ist auch grünes Prompten"
    Gutes Prompt Engineering (Kap. 14) spart nicht nur **deine Zeit**, sondern auch **Energie**: Wer sein Ziel in 1–2 präzisen Prompts erreicht statt in 15 vagen Versuchen, verursacht weniger Rechenlast. Qualität und Nachhaltigkeit gehen hier Hand in Hand.

---

## 36.5 Bewusste Nutzung mit Copilot

**Beispiel-Prompt zum Ausprobieren:**

```text
Erkläre den Unterschied im Energieverbrauch zwischen dem Training und der
Nutzung eines KI-Modells. Nenne anschließend drei konkrete Verhaltensweisen,
mit denen ich als Nutzer:in den Ressourcenverbrauch gering halte.
```

!!! info "Abwägung statt Verzicht"
    Es geht nicht darum, KI aus Umweltgründen zu meiden – sie kann ja selbst viel Ressourcen sparen (Kap. 29). Es geht um eine **ehrliche Abwägung** und **bewusste Nutzung**: KI dort einsetzen, wo sie echten Mehrwert schafft, und dabei effizient vorgehen.

---

## Zusammenfassung

- KI verbraucht real **Strom, Wasser und Rohstoffe** – über die Rechenzentren dahinter.
- **Training** ist einmalig sehr intensiv; **Nutzung** ist pro Anfrage klein, aber milliardenfach.
- Konkrete Verbrauchszahlen sind unsicher – zur **Sensibilisierung** nutzen, nicht als harte Fakten.
- Fußabdruck senken: grüne Energie, effiziente/kleine Modelle – und **bewusstes, effizientes Prompten**.
- **Effizientes Prompten** spart Zeit **und** Ressourcen; entscheidend ist die ehrliche Nutzen-Abwägung.

---

## Kurzübungen

{{ task(file="tasks/k36_01.yaml") }}

{{ task(file="tasks/k36_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k36.yaml") }}
