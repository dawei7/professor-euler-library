# CS.04 Maschinelles Lernen

License: CC BY-NC-ND 4.0 · Source: <https://doi.org/10.57813/20260220-092408-0> · 382 pages, 0 exercises in the prepared bundle

*Matthias Thimm*

## What this book trains

Matthias Thimms Maschinelles Lernen, erste Auflage 2026, ist Band 2 der Reihe hagen text books, erschienen bei Hagen University Press der FernUniversität in Hagen. Es folgt der klassischen Einteilung nach der Art der Erfahrung: überwachtes Lernen, unüberwachtes Lernen, Reinforcement Learning, dazu Deep Learning als Familie, die alle drei berührt. Am Anfang steht Mitchells Definition. Ein Programm lernt aus Erfahrung E bezüglich einer Klasse von Aufgaben T und eines Leistungsmaßes P, wenn seine Leistung bei T, gemessen mit P, mit E steigt.

Die Methode ist das durchgerechnete Beispiel. Kleine, oft ausdrücklich erfundene Datensätze werden Schritt für Schritt gerechnet: Körpergröße und Ringfingerumfang, Hund, Wolf und Dingo, Tennis und Temperatur, ein Staubsaugerroboter in zwei Räumen. Pseudocode hält die Algorithmen fest, von K-Means++ bis Backpropagation. Nummerierte Aufgaben druckt das Buch nicht. Das Bündel trägt deshalb das Buch und sein Inhaltsverzeichnis, aber keine markierten Aufgaben. Es ist ein Lesebuch: Man schreibt Notizen daneben oder rechnet ein Beispiel auf einem eigenen Blatt nach.

## Why it is worth knowing

Die lineare Regression ist das Muster für vieles danach. Setzt man den Gradienten des quadratischen Fehlers null, erhält man die besten Parameter in geschlossener Form, aber über die Inversion einer Matrix, die bei vielen Beispielen und Merkmalen teuer wird. Dann ist Gradient Descent der praktikable Weg. Dieselbe Kostenfunktion entsteht im Abschnitt über Bayes noch einmal, als Maximum-Likelihood-Hypothese unter normalverteilten Fehlern. Mit polynomiellen Merkmalen steigt das Bestimmtheitsmaß auf den Trainingsdaten mit jedem Grad. Auf den Testdaten steigt es typischerweise zuerst und fällt dann wieder. Das ist das Verzerrung-Varianz-Dilemma, und die Ridge-Regression begegnet der Überanpassung mit einem Strafterm auf die Quadrate der Parameter.

Der Kernel-Trick der Support Vector Machines berechnet ein Skalarprodukt im erweiterten Merkmalsraum, ohne die Merkmale aufzuschreiben. Der Informationsgewinn von ID3 bevorzugt Merkmale mit vielen Ausprägungen, im Extremfall das Datum, und C4.5 skaliert ihn deshalb. Die Hauptkomponentenanalyse sieht aus wie Regression und ist keine: Die Regression minimiert die vertikalen Abstände zur Geraden, die Hauptkomponentenanalyse die kürzesten, und die eine approximiert eine Funktion, die andere reduziert die Dimension. Ein einzelnes Perzeptron kann XOR nicht darstellen, geschichtete Perzeptronen können es. Die Freude an diesem Buch ist, jeden Schritt eines Verfahrens an einem Datensatz zu sehen, der auf eine Seite passt.

## What it asks of the other books

Das erste Kapitel wiederholt Notation, O-Notation, lineare Algebra, Analysis, Optimierung und Stochastik auf wenigen Seiten. Thimm sagt selbst, die Wiederholung sei absichtlich knapp und fixiere nur Begriffe und Notation, und fehlendes Wissen solle man sich anderswo aneignen. Gebraucht werden Matrizen, Eigenwerte und Eigenvektoren, partielle Ableitungen und der Gradient, bedingte Wahrscheinlichkeit und die Normalverteilung. Eine Fußnote sagt, dass mathematische Details abstrahiert und Voraussetzungen nicht immer geprüft werden. Programmcode enthält das Buch nicht.

Die erste Stufe des Pfads liefert diese Werkzeuge: Mathematics for Computer Science (CS.01) die O-Notation und die Wahrscheinlichkeit, Hefferon (03) die lineare Algebra bis zu den Eigenwerten, Calculus Volume 3 (06) die partiellen Ableitungen, den Gradienten und die Lagrange-Multiplikatoren. Grinstead und Snell (08) sind die gründlichere Wahrscheinlichkeit. Suh (24) erklärt die Dualität hinter dem dualen Problem der Support Vector Machines.

Im Pfad Computer Science & AI eröffnet Thimm die Stufe „Machine learning“, vor Prince (28) und Sutton und Barto (CS.05). Prince führt das Deep Learning weiter, das hier mit Autoencodern und Generative Adversarial Networks endet. Für das Reinforcement Learning empfiehlt Thimm selbst Sutton und Barto. Den Transformer nennt er nur im Ausblick, und Paaß und Giesselbach (CS.06) nehmen ihn in der letzten Stufe auf. Die Lerntheorie, die das Buch nach eigener Aussage kaum behandelt, steht in Bach (29), außerhalb dieses Pfads. Thimm und Marwedel (CS.02) sind die deutschen Bücher eines sonst englischen Pfads. Die im Katalog verzeichnete Lizenz ist CC BY-NC-ND 4.0, und das Impressum erteilt sie für den Text.

## A walk through the chapters

### Kapitel 1. Einleitung und Grundlagen

Kapitel 1, Einleitung und Grundlagen. Nach der Einleitung Notation und Multimengen, O-Notation, Matrizen bis zu Determinante und Eigenwert, Ableitung und Gradient, Gradient Descent und das Lagrange-Verfahren, Varianz, bedingte Wahrscheinlichkeit und Normalverteilung.

### Kapitel 2. Überwachtes Lernen

Kapitel 2, Überwachtes Lernen, ist das längste. Die lineare Regression führt die allgemeinen Begriffe ein: Bestimmtheitsmaß, Trainings- und Testdaten, Kreuzvalidierung, Über- und Unteranpassung, Regularisierung. Die logistische Regression klassifiziert trotz ihres Namens, gemessen durch Genauigkeit, Konfusionsmatrix, Präzision, Sensitivität und F1-Maß, und mehrere Klassen werden auf binäre Probleme zurückgeführt. Support Vector Machines legen eine Hyperebene, behandeln nicht linear separierbare Daten mit der Hinge-Kostenfunktion und mit Kernelfunktionen bis zur radialen Basisfunktion.

Die Nächste-Nachbarn-Klassifikation braucht kein Training im eigentlichen Sinn, aber viel Rechenzeit. Sie geht auch für Regression und macht die Merkmalskalierung wichtig. Der Bayes-Klassifikator beginnt beim Maximum-Likelihood-Prinzip und führt zur naiven Bayes-Klassifikation und zu kontinuierlichen Merkmalen. Entscheidungsbäume: ID3 mit Entropie und Informationsgewinn, C4.5, und Entscheidungswälder aus Bäumen, die auf Stichproben mit Zurücklegen gelernt werden und durch Mehrheit entscheiden.

### Kapitel 3. Unüberwachtes Lernen

Kapitel 3, Unüberwachtes Lernen. K-Means mit der Trägheit als Bewertung, der Ellenbogenmethode und K-Means++. Hierarchisches Clustering mit Dendrogrammen, agglomerativ als Single-Link-Clustering, divisiv als DIANA. Assoziationsregeln mit Support und Konfidenz, durch Apriori und FP-Growth. Anomalieerkennung durch Dichteabschätzung mit Normalverteilungen. Zuletzt die Hauptkomponentenanalyse.

### Kapitel 4. Reinforcement Learning

Kapitel 4, Reinforcement Learning, lehnt sich an Russell und Norvig an. Ein Markov-Entscheidungsprozess modelliert die Umgebung, und eine Strategie hat einen diskontierten Nutzen. Value Iteration und Policy Iteration bestimmen die optimale Strategie, wenn das Modell bekannt ist. Passives Reinforcement Learning schätzt Zustandsnutzen aus Probeläufen, durch adaptive dynamische Programmierung und Temporal Difference Learning. Aktives Reinforcement Learning sucht die Strategie selbst: Exploration gegen Exploitation, ε-greedy Learning, Q-Learning.

### Kapitel 5 und 6. Deep Learning, Zusammenfassung und Ausblick

Kapitel 5, Deep Learning, bleibt meist im überwachten Fall. Neuronen und Perzeptron, Feedforward-Netze, Aktivierungsfunktionen bis ReLU, Backpropagation, stochastischer und Mini-Batch-Gradient-Descent, das Problem des verschwindenden Gradienten. Convolutional Neural Networks mit Faltung, Padding, Stride und Pooling. Rekurrente Netze mit LSTM, bidirektionalen Netzen und einem Netz für automatische Übersetzung. Zuletzt Autoencoder und Generative Adversarial Networks.

Kapitel 6 fasst zusammen und nennt im Ausblick, was fehlt: die algorithmische Lerntheorie, Deep Reinforcement Learning und das Transformermodell. Literaturverzeichnis und Stichwortverzeichnis schließen das Buch.
