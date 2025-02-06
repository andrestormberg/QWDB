# Formulare anlegen und erweitern

**Lernen Sie Formulare anzulegen und zu bearbeiten. **

Die Struktur eines Formulars wird durch die Konfiguration der Zeilen und Spalten definiert. Zusätzlich können im Formular-Header (siehe Abbildung 1) Knotenpunkte oder "Filter" für Dimensionen ausgewählt werden, die nicht bereits in den Zeilen oder Spalten verwendet werden.



### Aufbau der Formulare


Vor dem Erstellen eines neuen Formulars müssen Sie zunächst festlegen, welche Daten im **Grid** *(auch als Raster oder Tabelle bezeichnet)* angezeigt werden sollen. Hierfür bietet Qvantum drei verschiedene Modi, die für die Konfiguration der **Zeilen** und **Spalten** verwendet werden können. Eine Beschreibung folgt weiter unten in diesem Artikel.


Es empfiehlt sich jedoch nicht, alle Dimensionen Ihres Modells in den Zeilen und Spalten zu platzieren, da dies bei der Vielzahl an Dimensionen schnell zu einem recht unübersichtlichen Formular führen würde. Dimensionen, die nicht im Grid liegen, stehen im **Formular Header**.  
  



![Abbildung 1 - Die Bestandteile eines Formulars](https://lp.qvantum-plan.de/hubfs/image-png-Sep-11-2023-08-15-06-7592-AM.png)


*Abbildung 1 - Die Bestandteile eines Formulars*


#### Der Formular-Header


Unabhängig von der Gestaltung Ihres Formulars gibt es höchstwahrscheinlich einige Dimensionen, deren aktuell ausgewähltes Element nur im Formular-Header (siehe Abbildung 1) ersichtlich ist. Diese Auswahl ist von großer Bedeutung, um zu verstehen, wofür die Zahlen im Raster stehen.


Ein Beispiel: Die Dimension "Jahre" befindet sich im Formular-Header und ist nicht Teil der Zeilen oder Spalten. Egal, welche Eingaben im Raster vorgenommen werden, es ist wichtig zu beachten, ob die Zahlen für das Jahr 2022 oder 2023 gelten.


### Formulare mithilfe des Formular-Grids anlegen


#### Konfiguration der Zeilen/Spalten


Über den Zeilen-/Spaltendialog (Abbildung 2) lassen sich die Inhalte für das Formular festlegen.


![Abbildung 2 - Konfiguration der Zeilen/Spalten](https://lp.qvantum-plan.de/hubfs/image-png-Aug-31-2023-12-29-02-6817-PM.png)


*Abbildung 2 - Konfiguration der Zeilen/Spalten*


### Modus festlegen


Zuerst legen Sie den Modus für Ihre Zeilen oder Spalten aus. Folgende Modi stehen zur Auswahl:


* Automatisch nach Dimensionen  
*Die Zeilen werden automatisch nach gewählten Dimensionen erzeugt.*
* Automatisch nach Ebenen  
*Die Zeilen werden automatisch nach den gewählten Ebenen (der ausgewählten Dimensionen) erzeugt.*
* Manuell  
*Die Zeilen werden einzeln von Ihnen manuell angelegt.*


Lassen Sie uns mit der einfachen dimensionstreuen Darstellung beginnen. 


### Automatisch nach Dimensionen


Sobald Sie eine Dimension ausgewählt haben, können Sie einen Knotenpunkt wählen, um die Dimension zu filtern (siehe Abbildung 3). Dabei werden nur die Elemente einbezogen, die sich unterhalb des ausgewählten Knotenpunkts befinden.


![Abbildung 3 - Dimension und Filter](https://lp.qvantum-plan.de/hubfs/image-png-Aug-31-2023-12-44-50-5880-PM.png)


*Abbildung 3 - Dimension und Filter*


 



Beachten Sie beim Hinzufügen einer zweiten Dimension die **Option "Leere Zeilen anzeigen"** *(siehe auch Abbildung 3)*. Nachdem Sie die erste Dimension festgelegt haben, ist Ausblenden der leeren Zeilen noch optional. Mit Hinzufügen der zweiten Dimension ist es nicht mehr möglich, alle leeren Zeilen automatisch einzublenden. 



### Automatisch nach Ebenen


Für die Konfiguration der Achse im Modus "Automatisch nach Ebenen" gestaltet sich der Dialog ein wenig anders. Anders als im Modus "Automatisch nach Dimensionen" kommt jetzt pro gewählter Dimension noch die Ebenenauswahl hinzu.


![Abbildung  4 - Konfiguration der Zeilen im Modus "Automatisch nach Ebenen"](https://lp.qvantum-plan.de/hubfs/image-png-Sep-11-2023-08-25-27-6090-AM.png)


*Abbildung  4 - Konfiguration der Zeilen im Modus "Automatisch nach Ebenen"*


Beim Anlegen der Struktur im Modus "Automatisch nach Ebenen", wählen Sie (1) eine Dimension, aus der Sie dann (2) eine Ebene auswählen (siehe auch Abbildung 4). Auf diese Art können Sie hierarchische Ebenen aus verschiedenen Dimensionen übereinander legen und eine grundlegend neue Struktur für Ihre Zeilen oder Spalten erstellen.


Um innerhalb der verwendeten Dimensionen und Ebenen bestimmte Bereiche zu filtern, können Sie die Kategorie **"Filter festlegen"** durch Anklicken öffnen. Dort werden die gerade erst für die Auswahl der Ebenen verwendeten Dimensionen gelistet. Pro Dimension können Sie einen Knotenpunkt auswählen, um nur diese Auswahl, inklusive seiner Kind-Elemente, im Formular auszugeben. 


 



**Achtung!**


Falls Sie eine oder mehrere Dimensionen nicht auswählen können, liegt das wahrscheinlich daran, dass die Ebenen noch nicht benannt wurden. Namen für Ihre Ebenen können Sie Ihrem Modell über die XLS-Konfigurationsdatei hinzufügen. Mehr zur Benennung der Ebenen finden Sie im [Artikel zur Konfiguration des Modells](https://lp.qvantum-plan.de/wissensdatenbank/modellvorlage#Ebenenname-im-Modell). 



### Manuell


**Hinzufügen von benutzerdefinierten Zeilen und Spalten**


Nachdem Sie die Dimensionen für die Spalten festgelegt haben, müssen Sie auf "Neue Zeile hinzufügen" bzw. "Neue Spalte hinzufügen" klicken, um konkret festzulegen, welche Zeile/Spalte angelegt wird.


In diesem Dialog zum Anlegen einer neuen Zeile/Spalte, stehen Ihnen außerdem **weitere Optionen** zur Verfügung. Es ist möglich, die Eingabe zu verbieten oder eine Kommentarzeile/-spalte einzublenden.


Wenn Sie die Eingabe verbieten, kann Ihr Planer in dieser Spalte keine Daten eingeben. Bei der Option "Kommentarzeile/-spalte einblenden" haben Sie die Wahl zwischen dem Kommentar-Typ "Freitext" oder "Freitext + Vorlage".


 


[![Abbildung 5 - Anlegen einer neuen Spalte im Modus "Manuell"](https://lp.qvantum-plan.de/hubfs/Imported%20images/formular_kommentar.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/formular_kommentar.png)


*Abbildung 5 - Anlegen einer neuen Spalte im Modus "Manuell"*


#### Vorlagen für die Kommentarspalte


Indem Sie den Kommentar-Typ "Freitext + Vorlagen" auswählen, können Sie dem Planer bestimmte Textbausteine vorgeben, welche er bei der Bearbeitung auswählen kann *(Abbildung 6)*.


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-12-2023-07-34-55-4400-AM.png)


*Abbildung 6 - Vorlagen für die Kommentarspalte*


Der Planer kann später Ihre Textvorlagen auswählen, indem er einen Doppelklick auf die Zelle durchführt und den entsprechenden Baustein auswählt *(Abbildung 7)*.


#### 


*Abbildung 7 - Auswahl Ihrer Textvorlagen für den Planer*


#### Berechnungszeile oder -spalte


Neben einer Datenspalte können Sie eine **Berechnungszeile/-spalte** in Ihr Formular einfügen. Geben Sie „Name der Zelle“/“Name der Spalte“ und die „Formel“ für die Berechnungszeile/-spalte an. Mehr zu Rechenoperationen und Formeln finden Sie [hier](https://lp.qvantum-plan.de/wissensdatenbank/rechenoperationen-und-formeln).


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Jan-25-2024-10-13-44-7817-AM.png)


*Abbildung 8 - Formeleingabe in einer Berechnungsspalte*


#### Wertetyp für Berechnungsspalten


Auch für Berechnungsspalten stehen die Wertetypen zur Verfügung, die in den [Grundeinstellungen von Qvantum](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-einstellungen) definiert sind. So können Sie sicherstellen, dass die berechneten Werte z.B. als Preise oder Prozentangaben ausgegeben werden. Über die Wertetypen lässt sich auch die Anzahl der Nachkommastellen bestimmen. Bei der Konfiguration einer Berechnungsspalte muss der gewünschte Wertetyp einfach zugewiesen werden.



Beachten Sie, dass es je nach Konfiguration eines Formulars auch dazu kommen kann, dass sich berechnete Zeilen und berechnete Spalten kreuzen. Wenn einer Zelle sowohl durch die Spalten- als auch durch die Zeilenkonfiguration ein Wertetyp zugewiesen ist, hat immer die Konfiguration der Spalte Vorrang.



 


**Option „Negative Werte hervorheben“**


Diese Option hebt alle negativen Werte (-1 und niedriger) im Formular rot hervor, die sich in dieser Zeile oder Spalte befinden.


 


 


 


 



**Category:** Formulare
**Subcategory:** Formulare anlegen
**Keywords:** Formel,Formularkopf,Formularraster,Grid,Spalten,Zeilen
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/formulare-anlegen)
