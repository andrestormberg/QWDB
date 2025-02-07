# Berechtigungen für verschachtelte Ebenen

**Formulare mit verschachtelten Ebenen unterliegen aufgrund ihrer speziellen Funktionalität bestimmten Regeln, die bei der Definition von Berechtigungen für Planer beachtet werden müssen.**


In diesem Artikel wird erläutert, wie die Berechtigungen für einen Planer und ein Formular mit verschachtelten Ebenen zusammenwirken. Die Nutzung des Formulars durch den Planer hängt sowohl von den ihm zugewiesenen Berechtigungen als auch von den verwendeten Ebenen im Formular ab. Informationen zur Erstellung eines Formulars mit verschachtelten Ebenen finden Sie in der [Kategorie Formulare](https://lp.qvantum-plan.de/wissensdatenbank/wie-baue-ich-ein-formular-mit-verschachtelten-ebenen). Abbildung 5 verdeutlicht aber den Zusammenhang zur Formularerstellung und zeigt, wie ein Formular mit verschachtelten Ebenen konfiguriert werden kann.



 


### Regel 1: Berechtigungen müssen auf der gleichen Ebene liegen


Damit ein Formular, das die verschachtelten Ebenen benutzt, für den Planer sichtbar ist, müssen die Berechtigungen auf Knoten der gleichen Ebene sitzen.


Im folgenden Beispiel (Abbildung 1) hat der Planer das Recht, die Region West und die Region Ost zu bearbeiten. Beide Knoten liegen auf Ebene 2 und das Formular wird für ihn angezeigt.


  


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-29-2023-09-34-03-4079-AM.png)


*Abbildung 1 - Der Planer hat die Berechtigung, sowohl auf die Knoten "Region West" als auch auf die Knoten "Region Ost" zuzugreifen.*


Im nächsten Beispiel ist der Planer berechtigt, "Region West" und "Hamburg" zu sehen. Die beiden Knoten liegen nicht auf der gleichen Ebene. Der Planer wird das Formular nicht benutzen können.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-29-2023-09-43-20-7451-AM.png)


*Abbildung 2 - Die Berechtigungen sitzen nicht auf der gleichen Ebene*


Um dem Planer das Formular zugänglich zu machen, müssen die Berechtigungen auf Städte-Ebene vergeben werden. Abbildung 3 zeigt, wie die Berechtigungen gesetzt werden, um das gleiche Resultat wie in Abbildung 2 zu erzielen.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-29-2023-09-47-18-8849-AM.png)


*Abbildung 3 - Alle Berechtigungen liegen auf der Städte-Ebene*


### Regel 2: Es darf keine Ebene im Formular verwendet werden, auf die der Planer nicht berechtigt ist


Die zweite Regel besagt, dass nur Ebenen verwendet werden dürfen, auf die der Planer berechtigt ist. Welche Ebenen das sind, lässt sich gut an Abbildung 4 erkennen. 


Da der Planer nur auf Knoten der dritten Ebene (Städte) berechtigt ist, kann Ebene 2 **nicht** für die Verschachtelung verwendet werden.


Ebenen 3 und 4 dürfen - auch einzeln (!) - in verschachtelten Formularen verwendet werden. Der Planer würde bei der Verwendung von Ebene 3 die Kunden 1-3 und 7-8 sehen, da diese unter den Knoten sitzen, auf die er berechtigt ist.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-29-2023-10-04-35-1853-AM.png)


*Abbildung 4 - Ebene 2 kann nicht für die Verschachtelung verwendet werden, da der Planer erst auf Knoten der dritten Ebene (Städte) berechtigt ist.*


 


*![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-29-2023-11-04-07-5730-AM.png)*


*Abbildung 5 - Bei der Konfiguration der Zeilen lassen sich im Modus "Automatisch nach Ebenen" nach Auswahl der Dimension, die einzelnen Ebenen auswählen.*


 



**Category:** Team
**Subcategory:** Nutzer-Berechtigungen
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/berechtigungen-für-verschachtelte-ebenen)
