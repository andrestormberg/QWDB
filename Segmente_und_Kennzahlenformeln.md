# Segmente und Kennzahlenformeln

**Lernen Sie, wie sie eine Segmentierung erstellen und die Kennzahlen in Ihrem Modell mit Formeln belegen können.**

Mit dem Formelmanager von Qvantum haben Sie die Möglichkeit, die Kennzahlen in Ihrem Modell einfach und effektiv mit Formeln zu verknüpfen. Wir unterstützen Sie bereits während der Formeleingabe mit einer Echtzeit-Validierung, die überprüft, ob die Formel im Modell gültig ist. 


Die nachfolgende Abbildung zeigt, wie sich die Ansicht unter *Modell > Formeln* zusammensetzt.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-36-30-3223-PM.png)


*Segmente (1) und die darin enthaltenen Kennzahlenformen (2)*



### **Segmente**


Lassen Sie uns zunächst klären, was mit dem Begriff „Segmente“ im Zusammenhang mit einem Datencube gemeint ist und welche Funktionen sie erfüllen.


Ein **Segment** ist ein definierter Teilbereich des Datenwürfels, der spezifische Daten anhand von Dimensionen (z. B. Varianten, Jahre) umfasst. Segmente werden genutzt, um Berechnungen und Formeln gezielt auf bestimmte Bereiche des Datenmodells anzuwenden, anstatt auf den gesamten Würfel.


#### Grund 1: Nicht rechnen


Formeln können in Qvantum für jede Kennzahl definiert werden. Ohne die Verwendung von Segmenten gilt jedoch eine Kennzahlenformel für den gesamten Datenwürfel. Stellen Sie sich vor, Sie importieren die IST-Werte des vergangenen Jahres aus einem anderen System in Qvantum, sei es manuell oder automatisiert über eine API. Anschließend stellen Sie fest, dass die angezeigten Werte in Qvantum nicht mit den hochgeladenen Werten übereinstimmen.


Der Grund dafür liegt in den Kennzahlenformeln, die auf den gesamten Würfel angewendet werden und somit die importierten Werte teilweise überschreiben können. Um dieses Problem zu vermeiden, können wir den Würfel in zwei Segmente aufteilen.


* **Die IST-Variante**: In diesem Segment soll keine Berechnung stattfinden.


* **Alle anderen Varianten**: Hier sollen Berechnungen durchgeführt werden.




Die folgende Abbildung veranschaulicht das Konzept dieser Segmentierung.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-12-49-03-2534-PM.png)


*Die Ist-Variante wird von den übrigen Varianten abgeschnitten*


#### Grund 2: Anders rechnen


Bestimmte Kennzahlen basieren auf Konstanten, die sich im Laufe der Zeit ändern können. Ein Beispiel hierfür könnte der durchschnittliche Sozialversicherungsbeitrag sein, der für die Planung des nächsten Jahres verwendet wird und jährlich angepasst wird. Für das Jahr 2025 möchten wir daher eine andere Konstante in die Berechnung integrieren als für 2024. Um diese Anpassungen vornehmen zu können, benötigen wir Segmente, die den Datenwürfel in Teilwürfel für die unterschiedlichen Jahre aufteilen.


### Das Schneiden von Segmenten


Um den zuvor aufgeführten Beispielen zu folgen, schauen wir uns jetzt an, wie wir den Datenwürfel entsprechend aufteilen.


In der linken Box „Segmente“ sehen wir bislang nur ein einziges Segment: den Datenwürfel, hier als „Komplettes Modell“ bezeichnet.


**Edit Modus**


Um Änderungen an der Segmentierung oder den Formeln vorzunehmen, müssen wir zuerst den Edit-Modus aktivieren, indem wir rechts oben auf „Edit“ klicken.


Wenn wir jetzt die Maus über ein Segment oder zu Beginn über das Komplette Modell in der Segmente Box bewegen, erscheint ein Plus Icon, um einen ersten Schnitt zu setzen. Die nachfolgende Abbildung zeigt den Vorgang.


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-12-50-49-3980-PM.png)


*Erst im Edit Modus kann eine neue Segmentierung erstellt werden.*


#### **Der erste Schnitt**


Nachdem Sie das Plus-Icon über dem kompletten Modell angeklickt haben, öffnet sich das Schnittfenster, in dem wir unseren ersten Schnitt entlang einer Dimension vornehmen können. In unserem Beispiel wählen wir zunächst die Dimension „Varianten“ aus, um den ersten Schnitt durchzuführen.


Jetzt haben wir die Möglichkeit, ein erstes Segment zu definieren. Wir benennen dieses Segment „IST-Variante“ und wählen im Dropdown-Menü rechts die entsprechenden Elemente aus der zuvor ausgewählten Dimension aus. In diesem Fall fügen wir lediglich das Element „Ist“ hinzu.


Bitte beachten Sie, dass die Dimension nach der Belegung des ersten Segments nicht mehr geändert werden kann, wie in der nachfolgenden Abbildung veranschaulicht wird.


 



Bitte beachten Sie, dass nur Elemente **aus der obersten Ebene der Hierarchie** einem Segment zugewiesen werden können.



 


**![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-12-53-49-6233-PM.png)***Im Schnittfenster können Segmente erstellt und Elemente zugewiesen werden.*


 


Beachten Sie, dass wir automatisch mit der Erzeugung des ersten Segments unter der Dimension „Varianten“ ein weiteres Segment „Restliche Varianten“ sehen können, welches unten ausgerichtet ist. Für unser Beispiel klicken wir nun auch schon auf „Anwenden“, um zur Hauptansicht zurückzukehren.


 



Bitte beachten Sie, dass Ihre Änderungen erst dann gespeichert werden, wenn Sie auf die Schaltfläche „Speichern“ oben rechts klicken.



 


Unser Modell wird nun, wie in der folgenden Abbildung zu sehen ist, deutlich dargestellt. Wir haben erfolgreich unser erstes Segment erstellt, und gleichzeitig wird das automatisch generierte Segment für die übrigen Elemente angezeigt.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-12-54-52-4452-PM.png)


*In der Hauptansicht wird der neue Schnitt mit seinen jeweiligen Elementen sofort dargestellt*


Im nächsten Schritt klicken wir in der Segmente-Box auf das neu erstellte Segment. Dadurch wird es hervorgehoben, und in der rechten Box erscheint die Überschrift:


Kennzahlen und Formeln für: Ist-Variante


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-12-58-19-9990-PM.png)


Der gesamte Inhalt der rechten Box bezieht sich auf das neu erstellte Segment „Ist-Variante“. Zunächst werden alle zuvor im Modell konfigurierten Formeln auch in diesem Segment angezeigt, jedoch sind sie hier lediglich „vererbt“.


Da wir im Segment „Ist-Variante“ keine Berechnungen vornehmen möchten und die importierten Daten unverändert bleiben sollen, ist es notwendig, die geerbten Formeln anzupassen. Dazu bewegen Sie im Editiermodus die Maus über eine Formel, wodurch ein Editier-Icon (Stift) erscheint. Durch einen Klick auf dieses Icon können Sie den Bearbeitungsmodus aktivieren. Die Formel wird dann im oberen Eingabefeld angezeigt, ähnlich wie in Excel.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-00-39-8474-PM.png)


Im Dropdown-Menü auf der linken Seite können Sie den Modus auswählen. Zur Verfügung stehen die Optionen: „Formel erben“, „Freie Formel“ und „Nicht rechnen“. Für unser Beispiel wählen wir die Option „Nicht rechnen“.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-00-50-6450-PM.png)


Das Eingabefeld für die Formel wird daraufhin geleert und ausgegraut, um anzuzeigen, dass keine Berechnung stattfindet. Klicken Sie auf „Übernehmen“ und wiederholen Sie diesen Vorgang für alle Formeln in diesem Segment. In der Kennzahlenbox wird jede erfolgreich geänderte Formel mit einer grünen Checkbox markiert, was bestätigt, dass die Änderung gültig ist.


#### Formel-Validierung


Beim Ändern von Formeln erfolgt eine sofortige Validierung Ihrer Eingaben in Echtzeit. Dadurch können Sie sofort feststellen, ob Fehler vorhanden sind. Solche Fehler können beispielsweise ungültige oder nicht existierende Schlüssel für andere Kennzahlen umfassen, die in der Formel verwendet werden. Zudem besteht die Möglichkeit, dass es zu Zykelbildungen kommt, was ebenfalls zu einem Fehler führen kann und dazu führen könnte, dass Ihre Änderungen nicht gespeichert werden.


### Der zweite Schnitt


Nachdem wir die Ist-Variante im ersten Schnitt erfolgreich als Teilwürfel definiert haben, der keine Berechnungen durchführt, wenden wir uns nun der zweiten Anforderung zu: In den verschiedenen Jahren sollen bestimmte Formeln mit unterschiedlichen Konstanten berechnet werden.


Um dies zu erreichen, betrachten wir erneut die Segmente-Box und fügen eine zweite Segmentierung unterhalb der „restlichen Varianten“ hinzu. Dazu klicken wir auf das Plus-Icon über dem Segment „restliche Varianten“, woraufhin das Schnittfenster geöffnet wird.


In diesem Schritt wählen wir die Dimension „Jahre“ aus. Anschließend erstellen wir für jedes Jahr, in dem abweichende Berechnungen erforderlich sind, separate Segmente. Diese Segmente werden dann entsprechend angeordnet und dargestellt.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-01-09-0781-PM.png)


Jetzt können die einzelnen Jahre unabhängig voneinander bearbeitet werden. Wenn Sie das gewünschte Segment auswählen, haben Sie die Möglichkeit, die Kennzahlenformeln spezifisch für jedes Jahr anzupassen. Hierzu müssen Sie lediglich die Formeln anpassen, die von den Standardberechnungen abweichen. Klicken Sie auf das Edit-Icon der entsprechenden Formel, um diese in das obere Eingabefeld zu übertragen. Ändern Sie anschließend den Modus von „Formel erben“ auf „Freie Formel“, nehmen Sie die erforderlichen Anpassungen vor und bestätigen Sie Ihre Eingaben mit „Übernehmen“.


#### Details zur Formelbearbeitung


In der nachfolgenden Abbildung wurde eine Formel über das Stift-Icon zur Bearbeitung ausgewählt. 


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-02-37-7494-PM.png)


*Das Eingabefeld zur Bearbeitung einer Formel*


Während Sie eine Formel bearbeiten, haben Sie die Möglichkeit, die Mouseover-Icons über den anderen Formeln in der Tabelle zu verwenden. Damit können Sie beispielsweise Kennzahlenschlüssel oder Teile anderer Formeln bequem in das obere Eingabefeld übertragen.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-02-56-3194-PM.png)


Kennzahlenschlüssel, die Sie über das Mouseover-Icon kopiert haben, können Sie einfach mit STRG+V in das obere Eingabefeld einfügen. Dabei werden die erforderlichen eckigen Klammern automatisch gesetzt, die für die korrekte Syntax unerlässlich sind.


Während Sie eine Formel bearbeiten, erfolgt kontinuierlich eine Überprüfung der Eingaben, sodass Sie sofort erkennen, ob die Formel gültig ist. Weitere Informationen zur korrekten Verwendung der Syntax finden Sie unter: [Rechenoperationen und Formeln](https://lp.qvantum-plan.de/wissensdatenbank/rechenoperationen).


Sobald Sie die Bearbeitung der Formel mit "Übernehmen" abgeschlossen haben, wird die bearbeitete Formel in der Liste in grüner Schrift angezeigt und erhält ein "Undo"-Symbol. Bitte beachten Sie, dass Ihre Änderungen erst gespeichert werden, wenn Sie auf den großen "Speichern"-Button oben rechts über der Tabelle klicken. Bis zu diesem Zeitpunkt haben Sie die Möglichkeit, bearbeitete Formeln über das Undo-Symbol zurückzusetzen.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-03-12-9595-PM.png)


*So erscheint eine bearbeitete Formel in der Liste*


 


Formeln, die in **grauer Schrift** dargestellt werden, sind **vererbt**, was bedeutet, dass sie von einem übergeordneten Segment abgeleitet sind. Diese Funktionalität reduziert den Aufwand für die Eingabe von Formeln erheblich, da nicht für jedes Segment alle Formeln neu eingegeben werden müssen. Stattdessen werden nur die Formeln angepasst und gespeichert, die spezifische Abweichungen für ein bestimmtes Segment aufweisen. Diese angepassten Formeln erscheinen dann in schwarzer Schrift.


![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-03-24-4120-PM.png)


#### Undo/Redo


**![](https://lp.qvantum-plan.de/hubfs/image-png-Nov-19-2024-01-03-35-2655-PM.png)**


Die Bearbeitung von Formeln wird durch eine Undo/Redo-Funktion unterstützt, die es Ihnen ermöglicht, Ihre Änderungen schrittweise zurückzusetzen. Dies gewährleistet Flexibilität und Kontrolle über Ihre Eingaben. Nachdem Sie alle gewünschten Anpassungen vorgenommen haben, können Sie diese durch einen Klick auf die Schaltfläche „Speichern“ dauerhaft sichern.



Bitte beachten Sie, dass solche Änderungen an Formeln oder Segmenten eine **vollständige Neuberechnung des Datenwürfels** erforderlich machen. Die Dauer dieses Prozesses kann je nach Größe und Komplexität Ihres Modells sowie der darin enthaltenen Daten variieren und entsprechend Zeit in Anspruch nehmen.



 


 



### Schematische Darstellung von Segmenten im Datenwürfel


Der mehrdimensionale Würfel basiert auf den von Ihnen angelegten Dimensionen. Um ein Verständnis für das Erstellen von Segmenten zu schaffen, ist im Folgenden ein 3-dimensionaler Würfel abgebildet. 


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Mar-12-2024-12-44-39-8456-PM.png)


*Der Datenwürfel mit den Dimensionen Jahren und Kennzahlen*


 


Bisher wird die Kennzahl "Sozialversicherung" anhand einer Formel berechnet. In dieser Formel ist eine Konstante enthalten, die zur Berechnung im Jahr 2023 geeignet ist. Für 2024 muss diese Konstante abgeändert werden. Es gibt also den Bedarf, im Jahr 2024 eine andere Kennzahlenformel zu hinterlegen als im Jahr 2023. 


Um das zu erreichen müsste der Würfel in Segmente für die Jahre 2023, 2024 und 2025 geschnitten werden. Erst wenn für das Jahr 2024 ein eigenes Segment geschaffen ist, kann eine abweichende Formel (und somit auch eine abweichende Konstante) hinterlegt werden.


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Mar-12-2024-12-45-23-3255-PM.png)


*Der Würfel wurde anhand der Dimension "Jahre" in 3 Segmente unterteilt*



**Category:** Modell
**Subcategory:** Formelmanager
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/segmente-und-formeln)
