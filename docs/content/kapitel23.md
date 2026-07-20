# Kapitel 23 – Praxis: KI in der Konstruktion

{{ progress(23) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Wie KI in **Konstruktion und Produktentwicklung** (CAD/Engineering) eingesetzt wird
- Was **generatives Design** ist und wie es sich vom klassischen Konstruieren unterscheidet
- Wie KI bei **Simulation, Varianten und Dokumentation** hilft
- Wo **Copilot** Konstrukteur:innen im Alltag unterstützt (Doku, Recherche, Kommunikation)
- Welche **Grenzen** (Sicherheit, Haftung, Prüfung) unbedingt gelten
</div>

---

## 23.1 KI in der Konstruktion – ein Überblick

Konstruktion und Produktentwicklung sind stark **wissens- und rechenintensiv**. KI setzt hier an mehreren Stellen an:

| Einsatzfeld | Was KI leistet |
|---|---|
| **Generatives Design** | erzeugt selbst Bauteil-Varianten nach Vorgaben |
| **Simulation** | schätzt Verhalten (Belastung, Strömung) schneller ab |
| **Varianten/Konfiguration** | passt Designs an Kundenanforderungen an |
| **Dokumentation** | erstellt Stücklisten, Berichte, Beschreibungen |
| **Wissenszugriff** | findet Normen, frühere Projekte, Bauteildaten |

---

## 23.2 Generatives Design

Beim **generativen Design** gibt der Mensch nur die **Ziele und Randbedingungen** vor – Material, Gewicht, Belastung, Bauraum – und die KI erzeugt daraus **automatisch viele mögliche Formen**, oft organisch anmutende, optimierte Strukturen.

```mermaid
flowchart LR
    A([Vorgaben: Last, Material, Bauraum, Gewicht]) --> B([Algorithmus erzeugt Varianten])
    B --> C([Bewertung: Festigkeit, Gewicht, Kosten])
    C --> D([beste Varianten zur Auswahl])
    D --> E([Ingenieur:in wählt & prüft])
```

!!! example "Klassisch vs. generativ"
    **Klassisch:** Der Ingenieur entwirft ein Bauteil und prüft, ob es hält. **Generativ:** Er definiert die Anforderungen, und die Software liefert **hunderte** optimierte Vorschläge – oft leichter und materialsparender, als ein Mensch sie entwerfen würde. Der Mensch wird vom **Zeichner** zum **Entscheider und Prüfer**.

!!! info "Wichtig"
    Generatives Design ist ein **Spezialwerkzeug** in CAD-Systemen (z. B. in Fusion, Siemens NX), nicht Teil von Copilot. Copilot ergänzt drumherum – bei Recherche, Doku und Kommunikation.

---

## 23.3 Wo Copilot Konstrukteur:innen hilft

Auch ohne CAD-Funktion entlastet **Copilot** die Konstruktionsarbeit erheblich – überall dort, wo **Text und Wissen** im Spiel sind:

| Aufgabe | Beispiel-Prompt |
|---|---|
| Anforderungen strukturieren | „Fasse dieses Lastenheft in klare, prüfbare Anforderungen." |
| Normen/Recherche | „Erkläre die Kernpunkte der Norm X in einfachen Worten." |
| Dokumentation | „Erstelle aus diesen Stichpunkten eine technische Beschreibung." |
| Kommunikation | „Formuliere eine verständliche Änderungsmitteilung an den Kunden." |
| Fehlersuche im Denken | „Welche Risiken übersehe ich bei dieser Konstruktionsentscheidung?" |

**Beispiel-Prompt zum Ausprobieren:**

```text
Ich habe folgende Kundenanforderungen an ein Bauteil: [Anforderungen].
Strukturiere sie in funktionale und nicht-funktionale Anforderungen, markiere
Widersprüche oder fehlende Angaben und formuliere 5 Rückfragen an den Kunden.
```

---

## 23.4 Grenzen und Verantwortung

!!! warning "Sicherheit geht vor"
    - **Technische Berechnungen und Festigkeitsnachweise** dürfen **niemals** ungeprüft aus KI übernommen werden – hier haften Menschen und Unternehmen.
    - Copilot kann bei **Normen und Formeln halluzinieren** (Kap. 15) – immer gegen die Originalquelle prüfen.
    - **Geistiges Eigentum:** Konstruktionsdaten sind oft hochsensibel; nur in freigegebener, geschützter Umgebung verarbeiten.
    - KI liefert **Vorschläge und Entwürfe** – die technische Verantwortung bleibt bei den Fachleuten.

!!! tip "Sinnvolle Arbeitsteilung"
    KI übernimmt das **Zeit- und Wissensmanagement** (Recherche, Struktur, Doku, Varianten), der Mensch die **fachliche und sicherheitsrelevante Entscheidung**. So gewinnt man Tempo, ohne die Verantwortung abzugeben.

---

## Zusammenfassung

- In der Konstruktion wirkt KI bei **generativem Design, Simulation, Varianten, Doku und Wissenszugriff**.
- **Generatives Design** kehrt die Arbeit um: Vorgaben rein, viele optimierte Varianten raus – Mensch entscheidet.
- **Copilot** entlastet vor allem bei text- und wissensbasierten Aufgaben rund um die Konstruktion.
- **Sicherheitsrelevante Berechnungen** und geistiges Eigentum erfordern strenge Prüfung und Schutz.

---

## Kurzübungen

{{ task(file="tasks/k23_01.yaml") }}

{{ task(file="tasks/k23_02.yaml") }}

{{ task(file="tasks/k23_03.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k23.yaml") }}
