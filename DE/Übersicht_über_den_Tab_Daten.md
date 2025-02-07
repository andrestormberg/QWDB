# Übersicht über den Tab Daten

**Daten importieren, exportieren und die Datenvorlage herunterladen.**



> 
> Der Tab „Daten“ ist nur für Benutzer mit der QVANTUM-Benutzerrolle „Controller“ verfügbar.
> 
> 
> 



Sobald Sie Ihre Modellvorlage hochgeladen haben, erhalten Sie im Tab Daten die Möglichkeit Ihre Daten zu [importieren](#importieren) oder [exportieren](#exportieren). Außerdem bietet QVANTUM Ihnen die Möglichkeit eine [Datenvorlage herunterzuladen](#herunterladen). 


Das  ["Änderungsprotokoll"](#changelog) bietet die Möglichkeit,  Änderungen an den Daten nachzuvollziehen. 


  
[![Tab Daten](https://lp.qvantum-plan.de/hubfs/Imported%20images/daten.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/daten.png)



### Importieren


Laden Sie die Daten (z.B. IST- oder historische Daten) hoch, die Sie in QVANTUM weiterverarbeiten möchten.


#### Hinweise zum manuellen Import von Daten


Laden Sie zunächst die auf Ihr Modell zugeschnittene Datenvorlage herunter und tragen Sie Ihre Daten zum Importieren ein. Anschließend können Sie die ausgefüllte Vorlage hochladen, wodurch die Daten im System gespeichert und entsprechend Ihres Modells weiterberechnet werden.  
  
Sie können jederzeit – auch während einer aktiven Planung – weitere Daten durch erneutes Hochladen hinzufügen. Bestehende Daten bleiben dabei erhalten, sofern Sie sie nicht überschreiben.



Sie können **xlxs-Dateien** mit einer Maximalgröße von **4MB** und **csv-Dateien** mit einer Maximalgröße von **1024MB** hochladen.




### Exportieren


Exportieren Sie die gesammelten Daten in ein Excel-kompatibles Format.


#### Hinweise **zum manuellen Export von Daten**


Durch Klicken auf den Button "Daten herunterladen" im Daten-Tab können Sie den Export Ihrer gesammelten Daten initiieren.  
  



![](https://lp.qvantum-plan.de/hubfs/image-png-Dec-02-2024-10-35-43-4126-AM.png)


Im ersten Schritt öffnet sich ein Dialog, in dem Sie den Umfang des Exports einschränken können. Wenn Sie die Daten in vollem Umfang herunterladen wollen, brauchen Sie hier keine weitere Auswahl zu treffen. Klicken Sie dann einfach auf "Exportieren".  
  



![](https://lp.qvantum-plan.de/hubfs/image-png-Dec-02-2024-10-37-51-2262-AM.png)


*Abbildung: Der Export-Dialog, in dem sich die Daten filtern lassen*


Um einen bestimmten Teil des Datencubes herunterzuladen, haben Sie die Möglichkeit, die gewünschten Elemente für jede Dimension auszuwählen. Dabei können Sie nur Elemente auf der untersten Ebene wählen, die über mehr als ein Element verfügen.


Angenommen, Sie möchten lediglich die Plandaten für das Jahr 2024 exportieren. In diesem Fall wählen Sie bei der Dimension "Jahre" die Option "2024" und bei der Dimension "Variante" das Element "Plan". Die anderen Dimensionen können Sie unverändert lassen, indem Sie die Auswahl auf "Alle Elemente" belassen.


![](https://lp.qvantum-plan.de/hubfs/image-png-Dec-02-2024-10-45-05-8980-AM.png)


*Abbildung: Filtern der Dimension "Jahre"*



Nach einem Export bleiben alle Daten weiterhin im System verfügbar und werden nicht gelöscht.



 



### Änderungsprotokoll/Changelog


Im Export-Bereich des Daten-Tabs erscheint ein Link "Änderungsprotokoll herunterladen". Darüber laden Sie alle Protokoll-Einträge im CSV Format-herunter. Die Datei kann z.B. mit Excel geöffnet werden.  


![](https://lp.qvantum-plan.de/hubfs/image-png-Jun-14-2023-08-27-24-2271-AM.png)


*Den Downloadlink für das Änderungsprotokoll finden Sie  im Exportbereich auf dem Daten-Tab*


 


Das Änderungsprotokoll erscheint mit englischen Spaltenüberschriften und ist wie folgt aufgebaut:


* **Time**  
Zeitpunkt an dem die Änderung vorgenommen wurde.
* **User**  
Der Benutzer, der die Änderung vorgenommen hat.
* **Type**  
Es gibt zwei unterschiedliche Arten von Änderungseinträgen:
	+ Change in cell value  
	Zellwertänderungen: Änderung an dem Wert, der in einer bestimmten Zelle sitzt.
	+ Data import  
	Eintrag, der darüber informiert, dass zu diesem Zeitpunkt ein Datenimport eingespielt wurde. **Achtung:** alle daraus resultierenden Zellwertänderungen werden nicht dokumentiert!
* **Bezugsspalten für jede Dimension**  
Für jede Dimension gibt es eine Bezugsspalte, in der festgehalten ist, auf welchem Element der Wert eingetragen ist.
* **Old value**  
In dieser Spalte steht der Wert, der vor der Änderung eingetragen war.
* **New value**  
Der neu eingetragene Wert.
* **Filename** (erscheint nur bei Einträgen der Art "Import")  
Der Dateiname der Datei, die importiert wurde.


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Jun-14-2023-10-01-01-4309-AM.png)


*Auszug aus dem Änderungsprotokoll*



### Datenvorlage herunterladen


QVANTUM stellt Ihnen eine Vorlage für Ihr Planungsmodell zur Verfügung. Dabei handelt es sich um eine Excel Datei, die Sie mit einem Klick auf „Datenvorlage herunterladen“ erhalten und dann entsprechend Ihren eigenen Wünschen ändern können.


  
[![Datenvorlage](https://lp.qvantum-plan.de/hubfs/Imported%20images/daten_vorlage-768x323.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/daten_vorlage-768x323.png)


#### Vorlage mit Daten füllen


Beim befüllen Ihrer Vorlage müssen Sie den Schlüssel, welchen Sie vorher im Modell bestimmt haben, eintragen.   
[![Daten Beispiel](https://lp.qvantum-plan.de/hubfs/Imported%20images/daten_beispiel.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/daten_beispiel.png)


 



**Category:** Daten
**Keywords:** Daten,Datenvorlage
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/tab-daten)
