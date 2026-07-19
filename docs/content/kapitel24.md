# Kapitel 24 – KI in der Produktion

{{ progress(24) }}

<div class="lernziele" markdown>
<h3>Was du in diesem Kapitel lernst</h3>

- Was **Industrie 4.0** und die **Smart Factory** bedeuten
- Welche Rolle KI in der modernen Produktion spielt
- Zentrale Einsatzfelder: Planung, Steuerung, Qualität, Wartung
- Welche Voraussetzungen (Daten, Vernetzung) nötig sind
</div>

---

## 24.1 Industrie 4.0 und Smart Factory

**Industrie 4.0** steht für die Vernetzung von Maschinen, Produkten und Systemen. In der **Smart Factory** kommunizieren Anlagen über Sensoren und liefern kontinuierlich Daten – die Grundlage für KI.

```mermaid
flowchart LR
    A([Sensoren / Maschinen]) --> B([Daten sammeln])
    B --> C([KI analysiert])
    C --> D([Optimieren & Steuern])
    D --> A
```

---

## 24.2 Einsatzfelder von KI in der Produktion

| Feld | KI-Nutzen |
|---|---|
| Produktionsplanung | Bedarf und Kapazitäten prognostizieren |
| Prozesssteuerung | Parameter automatisch optimieren |
| Qualitätssicherung | Fehler per Bilderkennung erkennen (Kapitel 25) |
| Instandhaltung | Ausfälle vorhersagen (Kapitel 26) |
| Logistik | Bestände und Wege optimieren |

!!! info "Datenbasis entscheidet"
    Produktions-KI lebt von **Sensor- und Maschinendaten**. Ohne verlässliche Datenerfassung (siehe Big Data, Kapitel 11) bleibt der Nutzen begrenzt.

---

## 24.3 Voraussetzungen und Grenzen

- **Vernetzung:** Maschinen müssen Daten liefern (nicht überall gegeben)
- **Datenqualität:** verlässliche, kontinuierliche Messwerte
- **Integration:** KI-Ergebnisse müssen in Steuerung/Abläufe zurückfließen
- **Sicherheit:** Produktionssysteme brauchen besonderen Schutz

**Copilot-Prompt zum Ausprobieren:**

```text
Erkläre am Beispiel einer Smart Factory, welche Daten für KI in der Produktion
nötig sind und nenne 4 konkrete KI-Anwendungen mit ihrem jeweiligen Nutzen.
```

!!! warning "Copilot ist nicht die Maschinensteuerung"
    Werkzeuge wie Copilot helfen bei **Planung, Auswertung und Dokumentation**. Die **Echtzeit-Steuerung** von Anlagen übernehmen spezialisierte Industrie-KI-Systeme.

---

## Kurzübungen

{{ task(file="tasks/k24_01.yaml") }}

{{ task(file="tasks/k24_02.yaml") }}

---

## Workshop

{{ task(file="tasks/workshop_k24.yaml") }}
