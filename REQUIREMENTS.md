# Python vs Science – Functional Programming & Lazy Evaluation

## Thema
**Funktionales Programmieren & Lazy Evaluation**

## Beschreibung
Python bietet Iteratoren und Generatoren, welche eine Form lazy basierter Datenverarbeitung ermöglichen. Diese Mechanismen stehen konzeptuell in Parallele zu LINQ in C# und erlauben die Verarbeitung großer bzw. unendlicher Datenmengen ohne signifikanten Speicherverbrauch.

## Wissenschaftliche Fragestellung
**"Speichereffizienz von Lazy Evaluation: Vergleich von Eager- vs. Lazy-Datenverarbeitung in Stream-Processing-Systemen."**

## Publikation
- *Functional Programming in Python*, David Mertz

## Beispielanwendung (Smart-Hive)
Verarbeitung endloser Nektar-Datenströme im *Honeybee Smart-Hive* zur Vermeidung von Speicherüberlauf.

---

# Aufgabe 6: RabbitFarm – Der Gemüsehof des Hasen

## Idee
Wie kann ein Hase Python nutzen, um einen nachhaltigen Gemüsehof zu betreiben und Waldtiere mit frischem Gemüse zu versorgen?

## Aufgabenstellung
Entwickeln Sie eine Python-basierte Anwendung, in der **Rudi der Hase** einen Gemüsehof gründet und mit Programmcode folgende Prozesse verwaltet:

- **Anbauflächen** (Gemüsesorten, Pflanzzeit, Erntezeitpunkt)
- **Lagerbestände** (Menge, Frische, Haltbarkeit)
- **Kundenbestellungen** (Abo-Kisten für Waldtiere)
- **Gewinne & Ausgaben** (Saatgut, Dünger, Wasserkosten)
- **Visualisierung von Erträgen** (Diagramme vergangener Saisons)
- **Objektorientierte Strukturierung**
  - Klassen für Gemüsesorten, Beete, Kunden, Lieferungen
- **Saisonale Angebote & Rezeptvorschläge**
  - Kreative Vorschläge sind erwünscht

---

# Wissenschaftlicher Fokus: Lazy Evaluation

## Fokuspunkt
Speichereffizienz der Lazy Evaluation im Vergleich zu Eager-Verarbeitung in datenintensiven Szenarien.

## Erweiterte Aufgabe
Verarbeiten Sie Sensordaten der Anbauflächen als **endlose Datenströme**. Nutzen Sie dazu:

- Python-Generatoren
- Die `itertools`-Bibliothek

Ziel ist es, Ernteerträge und Bewässerungspläne *lazy* zu berechnen, sodass nur die aktuell benötigten Daten im Speicher gehalten werden.

