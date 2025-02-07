# Eingabe in Formularen

**Erfahren Sie, welche Abkürzungen Sie bei der Eingabe von Zahlen verwenden können. Nutzen Sie unsere Zellfunktionen, um Werte bei der Eingabe automatisch zu berechnen.**

Als Planer müssen Sie sich nicht um die Einrichtung der Formulare kümmern. Ihr zentraler Controller hat sie bereits für Sie konfiguriert. Bevor Sie mit der Planung beginnen, sollte Ihnen Ihr Controller auch mitgeteilt haben, welche Formulare Sie bearbeiten müssen.  
  
In diesem Artikel erfahren Sie, wie Sie Daten in die Formulare eingeben und welche Funktionen Ihnen die Arbeit erleichtern.



### Zell Funktionen


Als Planer müssen Sie sich nicht um die Einrichtung der Formulare kümmern. Ihr zentraler Controller hat sie bereits für Sie konfiguriert. Bevor Sie mit der Planung beginnen, sollte Ihnen Ihr Disponent auch mitgeteilt haben, welche Formulare Sie bearbeiten müssen.  
  
In diesem Artikel erfahren Sie, wie Sie Daten in die Formulare eingeben und welche Funktionen Ihnen die Arbeit erleichtern.





| **Cell function** | **Syntax** | **Example** |
| Addieren | add<number>k
add<number>% | add5k (addiert 5,000)
add5% (addiert 5% vom Wert) |
| Subtrahieren | sub<number>k
sub<number>% | sub5k (subtrahiert 5,000)
sub5% (subtrahiert 5%) |
| Multiplizieren | mul<number> | mul5 (multipliziert mit 5) |
| Dividieren | div<number>
div<number>k | div5 (geteilt durch 5)
div5k (geteilt durch 5,000) |



 


Abbildung 1 veranschaulicht noch einmal die Verwendung von Tastaturkürzeln.


![](https://lp.qvantum-plan.de/hubfs/image-png-Apr-25-2024-04-37-13-7552-PM.png)


*Abbildung 1 - Hilfreiche Abkürzungen für die Eingabe Ihrer Planwerte.*



#### Zellfunktionen in andere Bereiche übertragen



Wenn Sie beispielsweise den Text „**add10%**“ markieren und ihn mit **STRG+C**(Kopieren) in die Zwischenablage kopieren, können Sie diese Funktion mit **STRG+V** (Einfügen) auf einen ausgewählten Bereich von Zellen anwenden.



### Weitere Funktionen auf dem Formular


Um bei einem großen Formular den Überblick zu behalten, haben Sie die Möglichkeit, Teile der Struktur auf- oder zuzuklappen. So können Sie sich bei der Bearbeitung nur die relevanten Zeilen oder Spalten anzeigen lassen, die Sie benötigen.


**Leere Zeilen und leere Spalten im Formular ausblenden**


Qvantum bietet auch die praktische Funktion, leere Zeilen oder Spalten nach Bedarf ein- oder auszublenden, unabhängig von der Achsenkonfiguration. Dazu finden Sie in der oberen rechten Ecke der Formulare ein Filtersymbol zum Ausblenden leerer Spalten. Das Symbol zum Ausblenden von Zeilen befindet sich unten links. Bitte beachten Sie, dass die Anzeige einer großen Anzahl von leeren Spalten oder Zeilen zu einer spürbaren Leistungseinbuße führen kann. Qvantum zeigt daher die Anzahl der ausgeblendeten Zeilen unten links im Formular an. Um die Anzahl der ausgeblendeten Spalten zu sehen, fahren Sie mit der Maus über das Filtersymbol oben rechts. Ein Mouseover-Tooltip zeigt Ihnen dann die genaue Anzahl an.


![](https://lp.qvantum-plan.de/hubfs/image-png-Mar-19-2024-10-38-29-2504-AM.png)


*Abbildung 2- Filter- und Dropdown-Funktionen im Formular*


 


Die folgenden Aktionen können darüber aufgerufen werden:


* **Alle aufklappen**Erweitert alle Knoten einer Struktur, so dass alle verfügbaren Zeilen/Spalten des Formulars angezeigt werden.
* **Alle komprimieren**Klappt alle Knoten einer Struktur zusammen, so dass nur die Wurzelelemente und Knoten der untersten Ebene angezeigt werden.
* **Leerzeilenfilter aktivieren**Wenn der Leerzeilenfilter aktiviert ist, werden nur Zeilen/Spalten angezeigt, die Werte enthalten. Dies verbessert die Übersichtlichkeit und blendet unnötige leere Bereiche aus.
* **Deaktivieren des Leerzeilenfilters**Wenn Sie den Leerzeilenfilter deaktivieren, werden alle Zeilen/Spalten angezeigt, auch wenn sie keinen einzigen Wert enthalten.


#### Verteilungsaktionen


In Strukturen ist es oft notwendig, die Werte aller untergeordneten Elemente in den Knoten zu summieren. Dies kann in verschiedenen Dimensionen notwendig sein. Befindet sich z.B. die Dimension 'Monate' im Formularkopf und ist der Knoten 'Gesamtjahr' ausgewählt, so müssen alle eingegebenen Werte auf die einzelnen Monate verteilt werden; in der Regel müssen Sie sich darum nicht kümmern, da Qvantum die Werte in der Zeitdimension automatisch gleichmäßig verteilt (jeder der 12 Monate erhält 1/12 des Wertes). Wenn jedoch ein Wert auf andere Zellen im Formular verteilt werden soll, ist es oft unklar, wie diese Verteilung erfolgen soll. In solchen Fällen fordert Qvantum eine Referenzspalte an, in der die Kindelemente des betreffenden Knotens bereits ausgefüllt sind.


#### Spaltenbreite ändern


Sie können die Spaltenbreite leicht anpassen. Bewegen Sie dazu die Maus zwischen den Spalten in der Kopfzeile und passen Sie die Breite per Drag'n'Drop nach Ihren Wünschen an.



Bitte beachten Sie, dass Änderungen an der Spaltenbreite nur vorübergehend erhalten bleiben. Wenn Sie sich das nächste Mal anmelden, wird das Formular in der vom zentralen Controller festgelegten Konfiguration neu geladen.



  
*![](https://lp.qvantum-plan.de/hubfs/image-png-Oct-30-2024-11-24-30-0467-AM.png)*


 


Bitte beachten Sie, dass Modelle, die vor März 2024 exportiert wurden, bald nicht mehr importiert werden können. Der Grund dafür ist die Formelspalte in der Dimension Kennzahlen, die den Import verhindert.



#### Sortieren von Wertespalten


Um eine Spalte auf- oder absteigend zu sortieren, bietet Qvantum im Spaltenmenü (drei Punkte Icon) die entsprechenden Aufrufe.


![](https://lp.qvantum-plan.de/hubfs/image-png-Jun-11-2024-07-52-47-9915-AM.png)


 



#### Filtern von Wertespalten


Im drei Punkte Menü, das an jeder Wertespalte verfügbar ist, können Sie einen Filter aktivieren. Folgende Filter sind hier verfügbar:


* Leer
* Nicht leer
* Gleich
* Ungleich
* Größer als
* Größer als oder gleich
* Kleiner als
* Kleiner als oder gleich
* Zwischen


Im Rahmen der hierarchischen Strukturierung von Elementen in Qvantum ist es von entscheidender Bedeutung, dass beim Filtern von Werten auch alle übergeordneten Zeilen des gefilterten Elements angezeigt werden. Dies gewährleistet, dass der Kontext des gefilterten Wertes erhalten bleibt. Daher kann es vorkommen, dass auch Werte angezeigt werden, die nicht den Filterkriterien entsprechen.


Im folgenden Beispiel ist es erforderlich, die Zeile „Support“ unabhängig von dem darin enthaltenen Wert anzuzeigen, um die Zuordnung der Mitarbeiter zu verdeutlichen.


 





| Struktur | **Filter aktiv (< 5.000€)**
Monatliche Gehälter |
| Vertrieb | 4.577,00€ |
|  | Peter Müller | 4.577,00€ |
| **Support** | **5.698,78€** |
|  | Petra Schmidt | 2.576,23€ |
|  | Frank Alster | 3.122,55€ |



*Beispiel für einen Filter, der nur Werte **unter** 5.000 in der Spalte anzeigt*


 


Der Filter kann über das 3-Punkte-Menü konfiguriert werden, das für jede Wertspalte verfügbar ist.


![](https://lp.qvantum-plan.de/hubfs/image-png-Oct-30-2024-10-37-57-7508-AM.png)


 



**Category:** QVANTUM für Planer
**Subcategory:** Vorbereitung vor Planungsbeginn
**Keywords:** Filter,forms
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/eingabe-in-formularen)
