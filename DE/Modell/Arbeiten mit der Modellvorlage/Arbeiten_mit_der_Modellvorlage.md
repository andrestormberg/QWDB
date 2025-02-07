# Arbeiten mit der Modellvorlage

**Definition und Upload des Planungsmodells, Dimensionseigenschaften und Dimensionen definieren.. **

Unsere Modellvorlage hilft Ihnen bei der Definition Ihres Modells anhand eines Beispiel-Vertriebsplans. In der folgenden Anleitung finden Sie eine detaillierte Schritt-für-Schritt-Anleitung.  
  
Wo Sie diese Datei finden, ist auf der Seite „[Modell](https://lp.qvantum-plan.de/wissensdatenbank/tab-modell)“ beschrieben.


### Aufbau der Modellvorlage


Die Excel-Modellvorlage unterteilt sich in viele Tabs (Arbeitsblätter), die hier im Folgenden beschrieben werden.


[![Die Blätter der Excel Modellvorlage](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-07-18-24-1185-AM.png)](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-07-18-24-1185-AM.png)


*Abbildung 1 - Die Excel-Modellvorlage ist in viele Arbeitsblätter zur Definition der einzelnen Dimensionen unterteilt*


Die Tabs im Detail:


* **Info**  
Auf diesem Reiter finden Sie weitere Hilfestellungen zur Verwendung dieser Vorlage.
* **Planungsmodell**  
Alle im Folgenden definierten Dimensionen (eine pro Arbeitsblatt) müssen hier gelistet sein. Außerdem muss jeder Dimension eine Rolle zugeordnet sein. Weitere Informationen zu den Rollen gibt es hier.
* **Dimensionen* (ein Blatt pro Dimension)**


### Planungsmodell


Ein Planungsmodell beschreibt eine Anwendung in Form eines multidimensionalen Würfels. Die Dimensionen des Würfels sollten dabei alle Aspekte Ihrer Planung abdecken. Hierdurch wird sichergestellt, dass Sie Ihre Daten unter Berücksichtigung aller benötigten Perspektiven und in diversen Detaillierungsstufen betrachten und bearbeiten können.


Jedes Datenelement (d.h. jede Zahl) in diesem multidimensionalen Würfel wird pro Dimension eindeutig einem Dimensionselement zugeordnet. Diese Dimensionselemente entsprechen somit anschaulich den Koordinaten einer Würfelzelle in der das Datenelement gespeichert wird.


Zunächst gilt es ein **Modellkürzel** und eine **Modellbezeichnung** festzulegen. Das Modellkürzel dient der eindeutigen Identifikation Ihrer Planung. Wenn Sie z. B. nachträglich die Bezeichnung Ihrer Planung ändern möchten, geschieht dies unter der Angabe dieses Kürzels. Die Modellbezeichnung ist der Name Ihres Planungsmodells. Sie wird in QVANTUM an verschiedenen Stellen angezeigt. **Modellbeschreibung**: hier können Sie eine ergänzende Beschreibung für Ihr Planungsmodell hinterlegen. Dieses Feld ist nicht verpflichtend.


[![](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-01-42-57-5564-PM.png)](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-01-42-57-5564-PM.png)


*Abbildung 2 - Der Tab "Planungsmodell" in der Modellvorlage*


Bevor wir uns den Tabs für die Dimensionen zuwenden, sollten Sie sich im Klaren sein, welche Dimensionen Ihre Planungsanwendung benötigt. Jede Dimension, die später auf einem eigenen Tab im Detail beschrieben wird, muss hier auf dem Tab „Planungsmodell“ gelistet sein. Dabei müssen die folgenden Spalten für jede verwendete Dimension befüllt werden:


* **Nummer**   
Die gelisteten Dimensionen müssen aufsteigend durchnummeriert sein (1-x). Die Nummer dient der eindeutigen Identifikation der Dimension im Planungsmodell. Wenn Sie z. B. nachträglich die Bezeichnung Ihrer Dimension ändern möchten, geschieht dies unter der Angabe dieser Nummer. Ihr Planungsmodell besteht aus verschiedenen Dimensionen.
* Die **Dimensionsbezeichnung**Die Dimensionen tauchen in QVANTUM an verschiedenen Stellen mit **Singular- oder Plural-Bezeichnung** auf. Hier können Sie die Bezeichnungen festlegen. Für jede Dimension müssen Sie ein weiteres Blatt in der Excel-Datei definieren. Dieses Blatt trägt den Pluralnamen der Dimension und dort können Sie Dimensionselemente definieren.
* Die **Dimensionsrolle***
* **Dimensionsbeschreibung**


Wenn Sie zu Beginn noch unsicher sind, welche Dimensionen in Ihrer Planung enthalten sind, können Sie sich auch zuerst den im Folgenden beschriebenen Dimensionsblättern zuwenden und zum Schluss wieder zum Tab "Planungsmodell" zurückkehren.



***) Dimensionsrollen**


Es gibt Dimensionen, die besondere Aufgaben in Ihrer Planung übernehmen. Diese Dimensionen werden über die Dimensionsrollen identifiziert. Folgende Dimensionsrollen gibt es:


**Kennzahlen (Pflichtangabe):** Die Dimension, die Ihre Kennzahlen identifiziert. Diese Rolle muss genau einer Dimension zugeordnet werden. Kennzahlen sind die quantitativen Inhalte die typischerweise im Controlling abgebildet werden, wie z. B. Absatzmengen, Erlöse, Kosten. Diesen Kennzahlen können sogenannte [Wertetypen](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-einstellungen) (Betrag, Prozentsatz, Preis, Menge, Bestand) zugeordnet werden, die auf dem Excel-Blatt zu dieser Dimension anzugeben sind. In dieser Dimension können außerdem Formeln zur Berechnung der jeweiligen Kennzahl hinterlegt werden. So könnte z.B. für die Kennzahl "Umsatz" die folgende Formel gelten:


Umsatz = Preis * Menge 


**Planungseinheiten (Pflichtangabe):** Die Dimension mit der Dimensionsrolle Planungseinheiten deckt den organisatorischen Aspekt einer Planung ab und steht oft im Zusammenhang mit Planungsverantwortlichkeiten für bestimmte Planungseinheiten, z. B. Bereiche, Filialen, etc. Diese Rolle muss genau einer Dimension zugeordnet werden. Merkmale, die in Planungseinheiten-Dimensionen erstellt werden, können später auch von den Planern bearbeitet werden. Merkmale anderer Dimensionen hingegen können nur von den Ownern/Controllern erstellt werden.


**Zeit (optional):** Diese Rolle können Sie genau einer Dimension mit Zeitcharakter zuordnen. Jahr- und Monatsdimensionen sind übliche Beispiele solcher Dimensionen. Möchten Sie mit Zeitversatzformeln arbeiten (z. B. Umsatz = Umsatz Vorjahr + 10%), so ist dies nur auf Dimensionen mit der Rolle Zeit möglich.


**Ohne besondere Rolle:** Diese Rolle können Sie allen übrigen Dimensionen zuordnen.



### Ein Tab für jede Dimension


Nachdem Sie den Tab "Planungsmodell" befüllt haben, muss sich für jede dort aufgeführte Dimension ein eigener Tab in der Modellvorlage befinden.


![](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-02-36-22-9674-PM.png)


 


Schauen wir uns nun an, anhand welcher **Spalten** die Elemente einer Kennzahlen-Dimension definiert werden.


![](https://lp.qvantum-plan.de/hubfs/image-png-Aug-11-2023-05-21-56-1332-AM.png)


*Abbildung 3 - Der Tab "Kennzahlen" in der Modellvorlage*


In der folgenden Abbildung sind die **Spalten** gelistet, mit denen eine Dimension beschrieben werden kann. Dabei wird grundsätzlich unterteilt in die Dimension "Kennzahlen" und alle übrigen Dimensionen.


#### 


#### Schlüssel


In dieser Spalte geben Sie den Schlüssel Ihrer Dimensionselemente ein. Schlüssel müssen nicht nur pro Dimension sondern innerhalb des ganzen Modells **eindeutig** sein. Eine als Schlüssel verwendete Zeichenkette darf also an keinem weiteren Element als Schlüssel verwendet werden.


#### Übergeordneter Schlüssel


Um hierarchische Dimensionen zu erhalten, können Sie in dieser Spalte für jedes Element ein übergeordnetes Element definieren. Dieses Element muss bereits vor der Verwendung oberhalb in der Tabelle als Schlüssel eingetragen worden sein. Verschiedene Elemente dürfen das selbe übergeordnete Element haben. 


In der folgenden Abbildung ist die Dimension "Monate" abgebildet. Ganz oben steht das Gesamtjahr, dem wir den Schlüssel "GJ" geben. Die einzelnen Quartale sitzen auf der zweiten hierarchischen Ebene und ihr übergeordneter Schlüssel heißt "GJ". Die Monate befinden sich auf der dritten hierarchischen Ebene. Der übergeordnete Schlüssel für die Monate Januar bis März wäre demnach "Q1".


 


[![Abbildung einer hierarchischen Struktur am Beispiel der Dimension "Monate"](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-33-31-1487-PM.png)](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-33-31-1487-PM.png)  
*Abbildung 4 - Eine hierarchische Struktur am Beispiel der Dimension "Monate"*


[![Abbildung der Dimension Monate aus der Modellvorlage](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-41-28-5789-PM.png)](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-41-28-5789-PM.png)


*Abbildung 5 - Die Dimension Monate aus der Modellvorlage*


  
Wollen Sie statt einer hierarchischen Dimension lieber eine flache Dimension haben, lassen Sie die Spalte „übergeordneter Schlüssel“ in jeder Zeile leer. So werden alle Elemente auf oberster Ebene angelegt.


#### Bezeichnung


In dieser Spalte können Sie die Bezeichnung Ihrer Elemente festlegen. 


[![Bezeichnung der Elemente in der Dimension Monate](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-47-04-4302-PM.png)](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-47-04-4302-PM.png)


*Abbildung 6a - Bezeichnung der Elemente in der Dimension Monate*


In den Formularen werden die Elemente später anhand ihrer Bezeichnung gelistet.


#### 


*Abbildung 6b - Die Elemente werden später im Formular anhand ihrer Bezeichnung erkannt.*


#### **Eingabe erlaubt?**


Hier können Sie für jedes Dimensionselement festlegen, ob hierzu im Planungsmodell Daten eingegeben werden dürfen.


[![Die Spalte "Eingabe erlaubt" in der Dimension Monate](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-49-01-4348-PM.png)](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-03-49-01-4348-PM.png)*Abbildung 7 - Die Spalte "Eingabe erlaubt" in der Dimension Monate*


**Hinweis**: Bitte beachten Sie, dass eine Dateneingabe im multidimensionalen Würfel des Planungsmodells nur möglich ist, wenn alle einer Würfelzelle zugeordneten Dimensionselemente bei „Eingabe erlaubt?“ die Einstellung „**Ja**“ besitzen. Wählen Sie die Einstellung „**Nein**“, wenn Sie sicherstellen wollen, das auf dem Dimensionselement unabhängig von der Kombination mit Elementen anderer Dimensionen grundsätzlich keine Eingabe erfolgen soll.  
  
Oft empfiehlt es sich, die Eingabe auf Knoten zu sperren, um die Planer zur Eingabe der Werte auf den unteren Elementen zu verpflichten. Indem Sie z.B. auf den Knoten "Quartal 1", "Erstes Halbjahr" und "Gesamtjahr" die Eingabe unterbinden, ist der Planer gezwungen, seine Zahlen auf Monatsbasis einzutragen.  
  
Beachten Sie, dass Kennzahlen, auf denen eine Formel eingetragen ist, keine Eingabe erlauben. Denn der durch die Formel berechnete Wert würde nach dem Speichern jede Eingabe wieder überschreiben.


Ein Element, auf dem grundsätzlich die Eingabe erlaubt ist, kann aber erst dann von einem Planer beschrieben werden, wenn es (a) ein Formular gibt, in dem sich das Element beschreiben lässt und (b) dem jeweiligen Benutzer nicht das Recht zum Beschreiben dieser Dimension/Elemente genommen wurde. Mehr zu den Benutzerrechten finden Sie [hier](https://lp.qvantum-plan.de/wissensdatenbank/nutzer-berechtigungen-in-qvantum-definieren).        



#### Wertetyp


Die Spalte Wertetyp gibt es nur auf dem Dimensions-Tab "Kennzahlen". Folgende Typen sind verfügbar: Betrag, Prozentsatz, Preis, Menge, Bestand. Wertetypen beschreiben, wie die Zahlen zu dieser Kennzahl formatiert werden. Sie können die Wertetypen in der Software konfigurieren. Hilfe dazu finden Sie [hier](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-einstellungen).


#### Beschreibung


In dieser Spalte besteht die Möglichkeit, zusätzlich eine Beschreibung pro Dimensionselement zu hinterlegen. Dieses Feld ist nicht verpflichtend.



#### Ebenenname


Die Befüllung der Spalte "Ebenenname" ist optional. Um in Formularen mit verschachtelten Ebenen arbeiten zu können, muss jede hierarchische Ebene einer Dimension, die dort verwendet wird, benannt sein. 



Die Dimension Monate kann z.B. hierarchisch in Gesamtjahr, Quartal und Monate unterteilt sein. Die drei hierarchischen Ebenen wären dann Gesamtjahr, Quartal und Monate. Es reicht aus, wenn jeweils das erste Element, das auf einer Ebene vorkommt, benannt wird.  


[![Bezeichnung der hierarchischen Ebenen](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-02-55-54-6946-PM.png)](https://lp.qvantum-plan.de/hubfs/image-png-Apr-24-2023-02-55-54-6946-PM.png)


*Abbildung 8 - Benennung der hierarchischen Ebenen*



#### Aggregation


Wenn Sie in dieser Spalte für ein Dimensionselement den Wert "Summe" auswählen oder das Feld leer lassen, wird dieses Element durch die Addition seiner untergeordneten Elemente berechnet. Das sind die Elemente, die diesem Element untergeordnet sind (zum Beispiel sind die Elemente "Januar", "Februar" und "März" dem Element "Quartal 1" untergeordnet).


Wenn Sie keine Addition wünschen, können Sie den Wert auf "Nicht aggregieren" setzen. 


Beachten Sie, dass die Aggregation in der Kennzahlen-Dimension über die Formelspalte definiert wird.



**ACHTUNG!**


In der Dimension "Kennzahlen" wird die Aggregationsregel in der Formelspalte festgelegt. Wenn Sie möchten, dass ein Knoten die Summe seiner untergeordneten Elemente enthält, tragen Sie in der Formelspalte die folgende Syntax ein:


**SumOfChildren()**



#### Formel


Formeln können nur in der Dimension mit der Rolle Kennzahlen vergeben werden. Folgende Rechenoperationen sind erlaubt:


* Addition (+)
* Subtraktion (-)
* Multiplikation (*)
* Division (/)
* SumOfChildren()


Wenn Sie auf andere Elemente der Kennzahlen-Dimension in einer Formel zugreifen möchten, setzen Sie den Wert vom "Schlüssel"-Feld des gewünschten Elements in eckige Klammern.



**Beispiel:** 


Kennzahl Erlöse = [VE]*[PPE]  
  **VE** = Schlüssel für "Verkaufte Einheiten"  
   **PPE** = Schlüssel für "Preis pro Einheit"



Weitere Informationen zur Verwendung von Formeln finden Sie [hier](https://lp.qvantum-plan.de/wissensdatenbank/rechenoperationen-und-formeln).


#### Alternative Formel für aggregierte Ebenen


In dieser Spalte können Sie optional eine Formel angeben, die statt der Formel in der Spalte "Formel" für all solche Zellen gerechnet werden soll, die für mindestens ein Dimensionselement einen Knoten mit darunterliegender Hierarchie adressieren. Die Formelsyntax ist dabei die gleiche wie für Formeln in der Spalte "Formel".



### Upload der Planungsanwendung


Wenn Sie diese Vorlage nach Ihren Anforderungen ausgefüllt und (unter einem eigenen Namen) als Excel-Modell-Datei gespeichert haben, können Sie zurück zur QVANTUM Web-Anwendung wechseln und diese Modelldefinition hochladen. Anschließend steht Ihnen das hochgeladene Modell zur weiteren Bearbeitung in der Cloud zur Verfügung.


**Die nächsten Schritte:**  
Sollte das in QVANTUM erzeugte Modell noch nicht Ihren (endgültigen) Anforderungen entsprechen, können Sie erforderliche Änderungen direkt in Ihre Excel-Datei einpflegen und den Upload wiederholen. Sofern Sie Daten (z.B. Ist-Daten vergangener Perioden) in das Modell übernehmen wollen, können Sie sich auf dem "Daten Tab"  eine zur Ihrem Modell passende Datenimportvorlage herunterladen, diese mit Daten befüllen und wieder hochladen.


[![Download der Datenvorlage auf dem Daten Tab](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-10-32-46-0314-AM.png)](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-10-32-46-0314-AM.png)


*Abbildung 9 - Download der Datenvorlage auf dem "Daten Tab"*


Entspricht das Modell Ihren Vorstellungen, so öffnen Sie Ihre QVANTUM Web-Anwendung und fahren Sie dort mit der Vorbereitung Ihrer Planung fort. Laden Sie Ihre Benutzer im Tab „Team“ hoch, die dann bei Start der Planung automatisch eine Mail mit einem Einladungslink erhalten.


Nach Erfassen der Plandaten durch die beteiligten Planer, können Sie die Planung in Qvantum beenden und Ihre Export-Berichte abrufen.


[![Beenden der Planung auf dem Reiter "Übersicht"](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-10-59-19-2344-AM.png)](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-10-59-19-2344-AM.png)


*Abbildung 10 - Beenden der Planung auf dem Reiter "Übersicht"*


[![Plandatenexport nach abgeschlossener Planung](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-10-54-44-4825-AM.png)](https://lp.qvantum-plan.de/hubfs/image-png-May-02-2023-10-54-44-4825-AM.png)


*Abbildung 11 - Plandatenexport nach abgeschlossener Planung*


Mehr zum Workflow über den "Übersichts-Tab" finden Sie [hier](https://lp.qvantum-plan.de/wissensdatenbank/uebersicht-workflow).


 



**Category:** Modell
**Subcategory:** Arbeiten mit der Modellvorlage
**Keywords:** Aggregation,Dimension,Formel,Modell,Modellvorlage
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/modellvorlage)
