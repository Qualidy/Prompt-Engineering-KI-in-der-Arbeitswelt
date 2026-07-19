# Kapitel 8 – Das KI-Periodensystem

{{ progress(8) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was das **KI-Periodensystem** ist und wozu es dient
- Die wichtigsten **Bausteine** (Fähigkeiten) von KI im Überblick
- Wie du damit passende **KI-Fähigkeiten** einem Problem zuordnest
- Wo **Copilot** in diesem Raster steht
</div>

---

## 8.1 Idee des KI-Periodensystems

Das **KI-Periodensystem** ist ein **Ordnungsraster**: Ähnlich wie das chemische Periodensystem Elemente sortiert, sortiert es die **grundlegenden Fähigkeiten** von KI. Es hilft, aus der Vielfalt der Begriffe eine klare Landkarte zu machen und für ein Problem die richtige „Zutat" zu finden.

!!! info "Kein starres Modell"
    Es gibt nicht *das eine* KI-Periodensystem – verschiedene Beratungen und Institute nutzen leicht unterschiedliche Varianten. Entscheidend ist die **Idee der Systematik**.

---

## 8.2 Die Bausteine (Fähigkeitsgruppen)

```mermaid
flowchart TD
    A([Wahrnehmen]) 
    B([Verstehen])
    C([Schlussfolgern])
    D([Handeln])
    E([Lernen])
```

| Fähigkeit | Bedeutung | Beispiel |
|---|---|---|
| Wahrnehmen | Sinnesdaten erfassen | Bild-/Spracherkennung |
| Verstehen | Bedeutung erschließen | Sprachverständnis (NLP) |
| Schlussfolgern | Aus Wissen ableiten | Empfehlungen, Diagnosen |
| Handeln | Aktionen ausführen | Roboter, KI-Agenten |
| Lernen | Aus Daten besser werden | Machine Learning |

---

## 8.3 Fähigkeiten einem Problem zuordnen

Vorgehen: Beschreibe die Aufgabe und frage, **welche Fähigkeit** benötigt wird.

| Aufgabe | Benötigte Fähigkeit(en) |
|---|---|
| Rechnungen automatisch auslesen | Wahrnehmen + Verstehen |
| Kundenanfrage beantworten | Verstehen + Schlussfolgern |
| Absatz prognostizieren | Lernen + Schlussfolgern |
| Maschine autonom steuern | Wahrnehmen + Handeln |

**Wo steht Copilot?** Copilot deckt vor allem **Verstehen** und (sprachbasiertes) **Schlussfolgern** ab – es versteht deine Anfrage und erzeugt passende Inhalte.

---

## 8.4 Anwendung mit Copilot

**Copilot-Prompt zum Ausprobieren:**

```text
Ich habe folgende Aufgabe: [Aufgabe beschreiben]. Welche grundlegenden
KI-Fähigkeiten (Wahrnehmen, Verstehen, Schlussfolgern, Handeln, Lernen) sind
dafür nötig? Begründe kurz und nenne je ein passendes KI-Verfahren.
```

---

## Kurzübungen

{{ task(file="tasks/k08_01.yaml") }}

{{ task(file="tasks/k08_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k08.yaml") }}
