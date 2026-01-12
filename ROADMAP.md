# RabbitFarm – Der Gemüsehof des Hasen

Projekt im Rahmen des Moduls **„Einführung in die Programmierung mit Python“**  
Thema 6: **RabbitFarm – Der Gemüsehof des Hasen** :contentReference[oaicite:0]{index=0}

---

## 1. Projektüberblick

Rudi, der Hase, betreibt einen nachhaltigen Gemüsehof und versorgt die Waldtiere mit frischem Gemüse.  
Die Python-Anwendung soll u. a. folgende Aufgaben unterstützen:

- Anbauflächen verwalten (Gemüsesorten, Pflanzzeit, Erntezeitpunkt)
- Lagerbestände überwachen (Menge, Frische, Haltbarkeit)
- Kundenbestellungen und Abo-Kisten verwalten
- Gewinne und Ausgaben erfassen
- Ernteerträge visualisieren
- Klassen für Gemüsesorten, Beete, Kunden und Lieferungen verwenden
- Saisonale Angebote und Rezeptvorschläge bereitstellen :contentReference[oaicite:1]{index=1}

---

## 2. Meilensteine (Portfoliophasen)

### 2.1 Konzeption (bis 26.01.2026 – Präsentation) :contentReference[oaicite:2]{index=2}

- [ ] Aufgabenstellung vollständig verstanden und abgegrenzt  
- [ ] Grobe Projektvision formuliert  
- [ ] Zielgruppe und Use Cases definiert  
- [ ] **Software Requirements** (funktional & nicht-funktional) formuliert und priorisiert  
- [ ] **Use-Case-Diagramm** / erste Skizzen erstellt (z. B. Mermaid in Markdown)  
- [ ] Benötigte Bibliotheken / Datensätze identifiziert  
- [ ] Konzeptdokument (3–5 Seiten) für PebblePad erstellt  
- [ ] Foliensatz für Konzeptpräsentation fertiggestellt  

### 2.2 Erarbeitung (bis 09.02.2026 – Präsentation) :contentReference[oaicite:3]{index=3}

- [ ] Python-Projektstruktur angelegt (z. B. `src/`, `tests/`, `data/`, `docs/`)  
- [ ] Minimale lauffähige App (MVP) erstellt  
- [ ] Mindestens **2 Software Requirements** prototypisch implementiert  
- [ ] Erste **Unit-Tests** und **Integrationstests** angelegt  
- [ ] Erste Dokumentation im Projekt (z. B. `docs/`, Docstrings) erstellt  
- [ ] Konzeption / Diagramme in Markdown (Mermaid/UML) integriert  
- [ ] Foliensatz für Erarbeitungspräsentation erstellt  
- [ ] Einarbeitungsdokumentation (Code + kurze Erläuterung) für PebblePad vorbereitet  

### 2.3 Finalisierung (März 2026 – Abgabe) :contentReference[oaicite:4]{index=4}

- [ ] Aufgabenstellung vollständig umgesetzt (oder klar dokumentierte Abweichungen)  
- [ ] Vollständiger Source Code inkl. benötigter Datensätze im Repo  
- [ ] **Developer-Wiki / Projektdokumentation** im Repo (Markdown)  
- [ ] Vollständige **README.md** (Setup, How-to-use, Features, Known Bugs, CI-Beschreibung)  
- [ ] **Software Requirements** final dokumentiert und auf Implementierung gemappt  
- [ ] **Software Design** (Use-Case, ggf. Sequenz-/Klassendiagramme) dokumentiert  
- [ ] **CI/CD-Konzept** und Testausführung dokumentiert (inkl. `requirements.txt`)  
- [ ] Mind. beispielhafte **Unit-Tests** und **3 Integrationstests** implementiert :contentReference[oaicite:5]{index=5}  
- [ ] 2-seitiger **Abstract / Reflexion** zur Projektdurchführung erstellt  
- [ ] Vollständiges Portfolio in PebblePad hochgeladen  

---

## 3. Funktionen & Features (Backlog mit Checklisten)

### 3.1 Datenmodell & Klassen

- [ ] Klasse `Vegetable` (Gemüsesorte, Sorte, Pflanzdatum, Erntedatum, Haltbarkeit, Menge)  
- [ ] Klasse `Bed` (Beet: Name, Fläche, Liste von Gemüsepflanzungen)  
- [ ] Klasse `Customer` (Kunde: Name, Adresse/Waldgebiet, Abo-Typ, Präferenzen)  
- [ ] Klasse `Order` (Bestellung: Kunde, Inhalt der Kiste, Lieferdatum, Status)  
- [ ] Klasse `Delivery` (Lieferung: Route, Kunde, Lieferstatus)  
- [ ] Klasse `Farm` (zentrale Verwaltung von Beeten, Lager, Kunden, Bestellungen)  

Für jede Klasse:

- [ ] Attribute definiert  
- [ ] Konstruktor und Methoden entworfen  
- [ ] Docstrings ergänzt  
- [ ] Mindestens ein Unit-Test pro Klasse erstellt  

---

### 3.2 Anbauflächen verwalten

- [ ] Funktion, um neue Beete anzulegen  
- [ ] Funktion, um Gemüse einer Anbaufläche zuzuordnen (Pflanzzeit, geplante Erntezeit)  
- [ ] Übersicht aller Beete mit aktuellem Anbauzustand  
- [ ] Filter/Abfrage nach Gemüsesorte, Beet oder Erntezeitpunkt  

Tests:

- [ ] Unit-Tests für Beetverwaltung  
- [ ] Integrationstest: „Beet anlegen → Gemüse pflanzen → Übersicht abrufen“  

---

### 3.3 Lagerbestände überwachen

- [ ] Datenstruktur für Lager (z. B. `Inventory`-Klasse oder Modul)  
- [ ] Erfassung von Menge, Frische, Haltbarkeit je Gemüsesorte  
- [ ] Funktion zum Auffüllen des Lagers nach Ernte  
- [ ] Funktion zur Bestandsprüfung (z. B. Warnung bei zu geringer Menge oder abgelaufener Haltbarkeit)  

Tests:

- [ ] Unit-Tests für Lagerlogik  
- [ ] Integrationstest: „Ernte → Lager → Bestellung“  

---

### 3.4 Kundenbestellungen & Abo-Kisten

- [ ] Kundendatenverwaltung (Anlegen, Bearbeiten, Löschen)  
- [ ] Abo-Typen definieren (z. B. „Basic-Kiste“, „Premium-Kiste“, „Karotten-only“)  
- [ ] Bestelllogik: Erstellen / Anzeigen / Stornieren von Bestellungen  
- [ ] Zuordnung von Gemüse aus dem Lager zu einer Bestellung  
- [ ] Einfache „Kisten-Vorschlagslogik“ auf Basis von Kundenpräferenzen  

Tests:

- [ ] Unit-Tests für Bestelllogik  
- [ ] Integrationstest: „Kunde → Abo → wiederkehrende Bestellung“  

---

### 3.5 Gewinne & Ausgaben

- [ ] Datenstruktur für Einnahmen (z. B. verkaufte Kisten)  
- [ ] Datenstruktur für Ausgaben (Saatgut, Dünger, Wasser, ggf. Personal)  
- [ ] Funktionen für einfache Gewinn- und Verlustrechnung (pro Zeitraum)  
- [ ] Ausgabe einer kleinen Finanzübersicht (z. B. Konsole oder Datei)  

Tests:

- [ ] Unit-Tests für Berechnungslogik  

---

### 3.6 Visualisierung der Ernteerträge

- [ ] Datenaufbereitung für Ernteerträge (z. B. pro Saison, pro Gemüsesorte)  
- [ ] Auswahl einer Visualisierungsbibliothek (z. B. `matplotlib`)  
- [ ] Erstellung von Diagrammen (z. B. Balken- oder Liniendiagramme)  
- [ ] Speicherung der Grafiken (z. B. `plots/`)  

Tests:

- [ ] Smoke-Test: Diagramm-Erzeugung ohne Fehler  

---

### 3.7 Saisonale Angebote & Rezepte

- [ ] Definition einer Datenstruktur für saisonale Angebote  
- [ ] Logik zur Bestimmung der Saison (z. B. einfache Monatslogik)  
- [ ] Vorschlagsfunktion für saisonale Kisten  
- [ ] einfache Sammlung von Rezeptideen basierend auf verfügbaren Gemüsesorten  
- [ ] Ausgabe der Vorschläge (Konsole, Datei oder einfache Textoberfläche)  

---

## 4. Technische Basis

- [ ] Entscheidung für Python-Version (z. B. `3.11`)  
- [ ] Anlage einer virtuellen Umgebung beschrieben (`venv` / `poetry` etc.)  
- [ ] `requirements.txt` gepflegt (für CI/Test)  
- [ ] Projektstruktur definiert und im README dokumentiert  

Beispielstruktur:

```text
rabbitfarm/
  src/
    rabbitfarm/
      __init__.py
      models/
      services/
      ui/
  tests/
  data/
  docs/
  plots/
  requirements.txt
  README.md
  PROJECT_PLAN.md
