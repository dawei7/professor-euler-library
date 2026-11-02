# CS.02 Eingebettete Systeme: Grundlagen Eingebetteter Systeme in Cyber-Physikalischen Systemen

License: CC BY 4.0 · Source: <https://doi.org/10.1007/978-3-658-33437-6> · 486 pages, 108 exercises in the prepared bundle

*Peter Marwedel*

## What this book trains

Peter Marwedels Eingebettete Systeme ist die zweite deutsche Auflage von 2021, übertragen aus der vierten englischen Ausgabe, und ein Lehrbuch für einen ersten Kurs über eingebettete und cyber-physikalische Systeme und das Internet der Dinge. Ein eingebettetes System ist ein informationsverarbeitendes System in einem umgebenden Produkt, etwa einem Auto oder einem Flugzeug. Ein cyber-physikalisches System betont die physischen Dinge, mit denen die Rechnung verbunden ist. Der Aufbau folgt einem Entwurfsfluss: Spezifikation, Hardware, Systemsoftware, Bewertung und Validierung, Abbildung von Anwendungen, Optimierung und Test.

Es ist keine Anleitung für einen bestimmten Mikrocontroller. Zeitverhalten, Speicherbedarf, Energie und Ausfälle gehören zur Aufgabe, nicht zur Nacharbeit. Am Ende jedes Kapitels stehen Aufgaben, 108 insgesamt, gedacht für zu Hause oder für die Präsenzphase eines flipped classroom. Viele fragen nach Begriffen. Andere verlangen einen Schedule, ein Petrinetz, einen A/D-Wandler oder eine Ausfallrate, einige eine Simulationssoftware oder eine Suche im Internet. Lösungen druckt das Buch nicht.

## Why it is worth knowing

Ein Ball, der bei jedem Aufprall einen festen Anteil seiner Geschwindigkeit verliert, springt im idealen Modell unendlich oft, und die Zeitpunkte der Stöße streben gegen eine endliche Zeit, weil die Reihe ihrer Abstände konvergiert. Das ist der Zeno-Effekt. Ein Digitalrechner kann unbegrenzt viele Ereignisse nur approximieren, so wie er reelle Zahlen nur approximiert. Hier trifft die Analysis auf die Maschine.

Eine Spezifikation wählt ein Berechnungsmodell: wie Komponenten rechnen und wie sie kommunizieren. Automaten, Datenfluss, Petrinetze und diskrete Ereignisse sind verschiedene Antworten, und keine passt auf alles. Ob die größtmögliche Ausführungszeit eines Programms endlich ist, ist im Allgemeinen unentscheidbar, als Folge des Halteproblems. Das Buch verlangt deshalb obere Schranken, die sicher und zugleich gut sind. Beim Rate Monotonic Scheduling halten periodische Tasks unter den Annahmen des Kapitels ihre Deadlines ein, solange ihre Auslastung eine Schranke nicht übersteigt, die mit der Zahl der Tasks gegen ln 2 fällt, etwa 0,7. Das Theorem vom kritischen Zeitpunkt gilt für einen Prozessor, nicht für mehrere, und deshalb werden die Beweise im Mehrprozessorfall wesentlich schwieriger. Die Freude an diesem Buch ist, eine Zeitgarantie als Satz zu lesen, dessen Voraussetzungen man prüfen kann.

## What it asks of the other books

Das Buch nennt seine Voraussetzungen selbst: Programmierung und erste Erfahrungen mit Mikrocontrollern, Algorithmen einschließlich der NP-Vollständigkeit, Rechnerorganisation mit endlichen Automaten, Grundlagen der Betriebssysteme und Rechnernetze, Mathematik wie Tupel, Integrale und lineare Algebra, dazu Elektrotechnik und Digitalschaltungen. Programmierung, Rechnerorganisation, Betriebssysteme, Rechnernetze und Elektrotechnik hat diese Bibliothek nicht. Wer sie nicht mitbringt, holt sie anderswo. Die Anhänge gleichen einige Lücken aus.

Aus der Bibliothek: Mathematics for Computer Science (CS.01) für Zustandsmaschinen, Graphen, partielle Ordnungen und Wahrscheinlichkeit. Calculus Volume 1 und 2 (02, 04) für Integrale und Reihen. Hefferon (03) für lineare Gleichungssysteme. Grinstead und Snell (08) für die Exponentialverteilung. Lebls Diffy Qs (13) für Differentialgleichungen und für die Fourier-Reihen, die das Buch nützlich nennt.

Im Pfad Computer Science & AI steht das Buch in der Stufe „Systems and robotics“, neben Elements of Robotics (CS.03). Marwedel nennt die Robotik selbst ein eng verwandtes Gebiet. Er empfiehlt auch, das Buch um einen Kurs über Datenanalyse oder maschinelles Lernen zu ergänzen. Im Pfad ist das die nächste Stufe, mit Thimm (CS.04). Die beiden sind die deutschen Bücher eines sonst englischen Pfads. Auf Englisch gibt es die offene vierte Ausgabe als Embedded System Design (Springer 2021). Sie gehört nicht zur Bibliothek. Die im Katalog verzeichnete Lizenz ist CC BY 4.0.

## A walk through the chapters

### Kapitel 1. Einleitung

Kapitel 1, Einleitung. Die Geschichte der Begriffe, Potential, Herausforderungen, gemeinsame Eigenschaften, die Einordnung in den Lehrplan, Entwurfsflüsse und die Struktur des Buches. Eingebettete Systeme sind meist reaktive Systeme, und deshalb sind endliche Automaten gute Modelle für sie. Das V-Modell und Gajskis Y-Diagramm erscheinen als Fälle eines iterativen Entwurfsflusses. 21 Aufgaben.

### Kapitel 2. Spezifikation und Modellierung

Kapitel 2, Spezifikation und Modellierung, ist das längste. Anforderungen, Berechnungsmodelle, frühe Entwurfsphasen bis zu Differentialgleichungen in Modelica, wo der springende Ball wiederkehrt. Kommunizierende Automaten mit StateCharts, synchronen Sprachen und SDL. Datenfluss mit Kahn-Prozessnetzwerken und SDF. Drei Arten von Petrinetzen. Die S-Invarianten eines Stellen/Transitions-Netzes sind Lösungen eines linearen Gleichungssystems. Ereignisbasierte Sprachen wie SystemC und VHDL, von-Neumann-Sprachen wie CSP und Ada, die Ebenen der Hardware-Modellierung und ein Vergleich der Modelle. 26 Aufgaben.

### Kapitel 3. Hardware eingebetteter Systeme

Kapitel 3, Hardware eingebetteter Systeme, folgt dem Signal durch die Schleife zwischen Umgebung und Rechner. Sensoren, Sample-and-hold, A/D-Wandler und das Abtasttheorem. Prozessoren, anwendungsspezifische Schaltkreise und rekonfigurierbare Logik. Speicherhierarchien bis zum Scratchpad-Speicher, Kommunikation mit Echtzeitgarantien. D/A-Wandler, Pulsbreitenmodulation, Aktuatoren. Elektrische Energie und sichere Hardware. 27 Aufgaben.

### Kapitel 4. Systemsoftware

Kapitel 4, Systemsoftware. Eingebettete Betriebssysteme und Echtzeitbetriebssysteme. Protokolle für den Zugriff auf Ressourcen: Prioritätsumkehr, Prioritätsvererbung, Priority Ceiling, Stack Resource Policy. ERIKA, Linux für eingebettete Systeme, die Hardware-Abstraktionsschicht, Middleware und Echtzeitdatenbanken. 12 Aufgaben.

### Kapitel 5. Bewertung und Validierung

Kapitel 5, Bewertung und Validierung. Pareto-Optimalität, größtmögliche Ausführungszeiten, der Realzeitkalkül, Qualitätsmetriken, Modelle des Energieverbrauchs und thermische Modelle. Verlässlichkeit, mit der Exponentialverteilung für Ausfälle: Bei konstanter Ausfallrate ist die mittlere Zeit bis zum Ausfall ihr Kehrwert. Fehlerbaumanalyse, Simulation, Emulation und formale Verifikation. 9 Aufgaben.

### Kapitel 6. Abbildung von Anwendungen

Kapitel 6, Abbildung von Anwendungen, ist das Kapitel über Scheduling. Für einen Prozessor Earliest Due Date, dessen Optimalität durch das Vertauschen zweier Jobs bewiesen wird, Earliest Deadline First, Least Laxity und Latest Deadline First, dann Rate Monotonic Scheduling für periodische Tasks. Für Multiprozessoren partitioniertes und globales Scheduling mit dem Dhall-Effekt, für abhängige Jobs ASAP, ALAP, List-Scheduling, ganzzahlige Programmierung, HEFT und evolutionäre Algorithmen. 4 Aufgaben.

### Kapitel 7 und 8, Anhänge

Kapitel 7, Optimierung, ist eine Auswahl: Schleifentransformationen, Festkomma statt Gleitkomma, Nebenläufigkeit von Tasks, Compiler, die Energie und Speicherarchitektur berücksichtigen, Spannungsskalierung und thermisches Management. 6 Aufgaben. Kapitel 8, Test, ist kurz: das Haftfehlermodell, Fehlersimulation und Fehlerinjektion, Scanpfad, Signaturanalyse und Pseudozufalls-Testmuster. 3 Aufgaben. Die Anhänge geben die ganzzahlige lineare Programmierung, die Kapitel 6 braucht, die Kirchhoffschen Gesetze mit dem Operationsverstärker für eine Schaltung aus Kapitel 3, und die Seitenadressierung mit Speicherverwaltungseinheiten.
