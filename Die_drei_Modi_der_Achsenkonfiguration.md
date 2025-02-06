# Die drei Modi der Achsenkonfiguration

**Dieser Artikel beschreibt das Verhalten des jeweiligen Modus  bei der Konfiguration der Spalten oder Zeilen.**

Beim Konfigurieren der Zeilen oder Spalten muss zunächst festgelegt werden, in welchem Modus die Achse konfiguriert werden soll. Folgende Modi stehen zur Auswahl:  

1. [Automatisch nach Dimensionen](#Automatisch-nach-Dimensionen)
2. [Automatisch nach Ebenen](#Automatisch-nach-Ebenen)
3. [Manuell](#Manuell)


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-04-2023-10-27-57-7052-AM.png)


*Abbildung 1 - Der Modus im Dialog zu Konfiguration der Zeilen/Spalten*


Um das Verhalten des jeweiligen Modus anhand von Beispielen zu erklären, sind zunächst zwei Beispieldimensionen abgebildet, die in den meisten Modellen verwendet werden: Jahre und Monate.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-01-2023-07-33-28-8017-AM.png)


*Abbildung 2 - Die Dimensionen Monate (links) und Jahre (rechts)*



### Automatisch nach Dimensionen


Im Modus "Automatisch nach Dimensionen" werden die gewählten Dimensionen nach dem folgenden Prinzip ineinander verschachtelt: 


Die Struktur der zuerst gewählten Dimension wird dargestellt. Für jedes Element auf der untersten Ebene wird nun die Struktur der darauf folgenden Dimension integriert. Im Beispiel mit den Monaten und Jahren bedeutet dies, dass wir zuerst die Struktur der Dimension Monate sehen, die Quartale und darunterliegende Monate umfasst. Unter jedem Monat, also auf der untersten Ebene, wird nun die vollständige Dimension "Jahre" untergliedert. In Abbildung 2 ist zu erkennen, dass diese Dimension nur die Elemente 2022, 2023 und 2024 enthält, da keine weiteren Elemente darunter platziert sind.


In Abbildung 3 ist zu sehen, wie die Strukturen der Dimensionen Monate und Jahre verschachtelt werden.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-01-2023-07-37-46-2985-AM.png)


*Abbildung 3 - Prinzip des Modus "Automatisch nach Dimensionen"*


 


Konfigurieren wir die Zeilen in unserem Formular allerdings nach diesem Muster (*siehe Abbildung 4*), zeigt sich, dass im Formular nur die 'Blätter' angezeigt werden.  Damit sind alle Elemente gemeint, auf denen Werte eingetragen werden können. In der Dimension 'Monate' wären das die Monate (Ebene 2), denn bei den Quartalen handelt es sich **nicht** um Blätter sondern um Knoten (z.B. '1. Quartal'), auf denen alle darunter liegenden Elemente (für '1. Quartal' wären das 'Januar', 'Februar', 'März') aufsummiert werden.   


*![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-04-2023-08-43-50-4783-AM.png)*


*Abbildung 4 - Die Konfiguration der Zeilen im Modus "Automatisch nach Dimensionen"*


 


Nach dieser Konfiguration (Abbildung 4) wird das Formular anschließend wie folgt (Abbildung 5) dargestellt.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-04-2023-09-35-42-2315-AM.png)


*Abbildung 5 - Die Blattverschachtelung im Modus "Automatisch nach Dimensionen"*


 



Im Modus "Automatisch nach Dimensionen" werden beim Verschachteln von zwei oder mehr Dimensionen nur noch die Zellen angezeigt, in denen Werte stehen.  




### Automatisch nach Ebenen


Es ist zunächst wichtig zu verstehen, was mit "Ebenen" gemeint ist. In der Dimension "Monate" werden zwei hierarchische Ebenen verwendet: Quartale (Ebene 1) und Monate (Ebene 2). Im Gegensatz dazu gibt es in der Dimension "Jahre" nur eine Ebene, auf der die Elemente 2022, 2023 und 2024 platziert sind. Mit Ebene ist im Zusammenhang mit der Verschachtelung immer die hierarchische Ebene einer Dimension gemeint.



Qvantum ermöglicht es, diese Ebenen direkt im Modell zu benennen, was es später einfacher macht, die entsprechende Ebene bei der Verschachtelung auszuwählen.



Im Modus "Automatisch nach Ebenen" können jetzt z.B. die Dimensionen "Monate" (mit den Ebenen "Quartale" und "Monate") und "Jahre" (mit der Ebene "Jahre") zu einer neuen Struktur verschachtelt werden (siehe Abbildung 6).  
  
![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-01-2023-07-48-05-6211-AM.png)


*Abbildung 6 - Das Prinzip des Modus "Automatisch nach Ebenen"*


Die Konfiguration der Zeilen stellt sich damit wie folgt (Abbildung 7) dar.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-04-2023-10-16-01-1194-AM.png) 


*Abbildung 7 - Konfiguration der Zeilen im Modus "Automatisch nach Ebenen"*


Werfen wir einen Blick auf das Formular, welches nun generiert wird. Es fällt auf, dass bei dieser Verschachtelung keine Werte für die Quartale ermittelt werden können. Denn bei diesem Formularaufbau gibt es für die Quartale keinen Bezug zum Jahr.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-04-2023-10-21-02-5090-AM.png)


*Abbildung 8 - Die Darstellung der zuvor verschachtelten Ebenen im Formular*
### Manuell


Im Modus "Manuell" können in beliebiger Reihenfolge Dimensionen ausgewählt werden, ähnlich wie im Modus "Automatisch nach Ebenen". Nach dem Speichern der Konfiguration wird jedoch noch keine Zeile oder Spalte erstellt. Dies muss anschließend manuell entsprechend der erstellten Konfiguration erfolgen.


**Beispiel**


In einer manuellen Spaltenkonfiguration wurden die Dimensionen Jahre und Monate ausgewählt (siehe Abbildung 9). Im Anschluss können Sie nun über das Plus Icon Spalten manuell hinzufügen. Der Dialog gestaltet sich so, wie in Abbildung 10 zu sehen.


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-01-2023-11-15-30-4936-AM.png)


*Abbildung 9 - manuelle Spaltenkonfiguration*


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-01-2023-11-20-40-5451-AM.png)


*Abbildung 10 - Hinzufügen einer Spalte zu manuellen Spaltenkonfiguration*



**Category:** Formulare
**Subcategory:** Weiteres zu den Konfigurationsmöglichkeiten
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/die-drei-modi-der-achsenkonfiguration)
