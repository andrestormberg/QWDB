# Glossar: Alle relevanten Begriffe rund um den Datencube auf einen Blick

**Dieses Glossar erklärt die wichtigsten Begriffe, die im Kontext der Qvantum Wissensdatenbank und rund um den Datencube verwendet werden.**


**Achsen im Formular**  
Formulare in Qvantum basieren auf den Achsen des Datencubes. Jede Achse repräsentiert eine Dimension, und die Felder eines Formulars werden entlang dieser Achsen angeordnet. Ein Planer könnte beispielsweise eine Kostenstelle (Spaltenachse) über verschiedene Zeiträume (Zeilenachse) planen.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/formulare-anlegen)


 


**Aggregation**  
Aggregation bezeichnet die Zusammenfassung von Daten auf einer höheren Ebene. So können z.B. die Gehälter der Mitarbeiter unter dem Knoten "Vertrieb" auf der Ebene "Abteilungen" aufsummiert werden. In Qvantum ist der "Durchschnitt" nur über einen Workaround verfügbar, da er nicht als Aggregationsregel hinterlegt ist.   
[Qvantum Wissensdatenbank, Aggregationsfunktionen](https://lp.qvantum-plan.de/wissensdatenbank/modell)


 


**Änderungsprotokoll (Changelog)**  
Das Änderungsprotokoll bietet eine Übersicht über alle vorgenommenen Änderungen an den Daten im Datencube. Es enthält Informationen darüber, wer welche Änderung zu welchem Zeitpunkt durchgeführt hat und kann als CSV-Datei exportiert werden.  
[Qvantum Wissensdatenbank, Tab „Daten“](https://lp.qvantum-plan.de/wissensdatenbank/tab-daten)


 


**API (Application Programming Interface)**  
Eine API ermöglicht es, Softwarekomponenten miteinander zu kommunizieren. Sie wird verwendet, um Daten zwischen externen Systemen zu übertragen oder zu verarbeiten.  
[Qvantum Wissensdatenbank, API-Dokumentation](https://api.qvantum-plan.de/tutorial/index.html)


 


**Authentifizierung**  
Authentifizierung bezeichnet den Prozess der Verifizierung eines Benutzers oder Systems, um Zugriff auf bestimmte Daten oder Funktionen zu gewähren. Dies sorgt dafür, dass nur berechtigte Nutzer auf die entsprechenden Daten zugreifen können.


**Benutzerrechte**  
Benutzerrechte steuern den Zugriff auf Daten innerhalb des Datencubes. In Qvantum können Benutzerrechte so konfiguriert werden, dass Planer nur auf bestimmte Teilwürfel zugreifen können, basierend auf ihrer Rolle oder ihren Verantwortlichkeiten.  
[Qvantum Wissensdatenbank, Nutzer-Berechtigungen](https://lp.qvantum-plan.de/wissensdatenbank/guide-nutzerberechtigungen-vergeben)


 


**Datenexport**  
Datenexport bezeichnet den Vorgang, bei dem Planungsdaten aus Qvantum in externe Systeme oder Formate (z. B. Excel) exportiert werden. Dies ermöglicht es den Benutzern, die Daten außerhalb des Systems weiter zu bearbeiten oder Berichte zu erstellen.  
[Qvantum Wissensdatenbank, Tab „Daten“](https://lp.qvantum-plan.de/wissensdatenbank/daten)


 


**Datenimport**  
Datenimport ist der Prozess des Einlesens externer Daten in den Qvantum-Datencube. Dies erlaubt es Nutzern, vorhandene Datenquellen wie Excel-Dateien oder andere ERP-Systeme zu integrieren, um sie für Planungszwecke zu nutzen.  
[Qvantum Wissensdatenbank, Tab „Daten“](https://lp.qvantum-plan.de/wissensdatenbank/daten)


 


**Dimensionselement**  
Ein Dimensionselement ist eine spezifische Ausprägung innerhalb einer Dimension, wie z.B. ein bestimmtes Jahr in der Dimension *Jahre* oder eine Kostenstelle in der Dimension *Organisationseinheiten*.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-f%C3%BCr-planer)


 


**Dimensionsrollen**  
Dimensionsrollen geben einer Dimension eine spezielle Bedeutung und steuern, wie die Daten innerhalb dieser Dimension verarbeitet werden. Zum Beispiel hat die Dimension *Jahre* die Rolle der Zeitdimension. Wenn in einem Formular beispielsweise ein Jahresgehalt eingetragen wird, kann durch die Zeitrolle der Dimension eine automatische Verteilung des Gehalts auf die 12 Monate des Jahres erfolgen.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-f%C3%BCr-planer)


 


**Drill-Down**  
Der Drill-Down ist die Möglichkeit, von einer aggregierten Ansicht auf detailliertere Daten herunterzubrechen. In Qvantum könnte ein Planer von einer Gesamtvertriebszahl auf die Umsätze pro Region oder sogar pro Kunde drillen.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-f%C3%BCr-planer)


 


**Formulardefinitionen exportieren und importieren**  
Formulardefinitionen können in Qvantum exportiert und importiert werden, um Formularstrukturen zwischen verschiedenen Systemen zu übertragen. Dies erfolgt im JSON-Format und ist besonders nützlich für Backups und den Transfer von Formularkonfigurationen.  
[Qvantum Wissensdatenbank, Export und Import von Formulardefinitionen](https://lp.qvantum-plan.de/wissensdatenbank/formulardefinitionen-exportieren-und-importieren)


 


**Formular**  
Ein Formular in Qvantum ist die Schnittstelle, über die Planer ihre Daten in den Datencube eingeben. Formulare sind vom Owner vorbereitet und enthalten Felder, die auf den Dimensionen des Datencubes basieren. Sie definieren, welche Daten der Planer eingeben kann und welche Daten nur angezeigt werden.  
[Qvantum Wissensdatenbank, Arbeiten mit Formularen](https://lp.qvantum-plan.de/wissensdatenbank/formulare#arbeiten-mit-formularen)


 


**Formularkonfigurationen**  
Qvantum ermöglicht es, Formulare nach den Anforderungen des Benutzers zu konfigurieren. Dies umfasst die Anpassung von Layouts, die Definition von zugänglichen Feldern und die Festlegung von Berechtigungen für die Eingabe.  
[Qvantum Wissensdatenbank, Weiteres zu den Konfigurationsmöglichkeiten](https://lp.qvantum-plan.de/wissensdatenbank/formulardefinitionen-exportieren-und-importieren)


 


**Grid Formatierung**  
Die Grid-Formatierung in Qvantum ermöglicht es, Formulare visuell anzupassen, um Planern eine übersichtliche Darstellung der Daten zu bieten. Dies umfasst z. B. die Anpassung von Farben, Schriftarten oder Zellgrößen.  
[Qvantum Wissensdatenbank, Arbeiten mit Formularen](https://lp.qvantum-plan.de/wissensdatenbank/grid-formatierung)


 


**Hierarchie**  
Hierarchien ordnen die Elemente einer Dimension auf unterschiedlichen Ebenen an. Zum Beispiel könnte die Dimension *Organisationseinheiten* eine hierarchische Struktur haben, die von einer globalen Organisationseinheit bis hin zu spezifischen Unterorganisationseinheiten reicht.


**Kennzahl**  
Kennzahlen befinden sich immer in der Dimension *Kennzahlen*. Diese Dimension hat auch die spezielle Rolle *Kennzahlen*. Eine Besonderheit dieser Dimension in Qvantum ist, dass Kennzahlen mit Formeln definiert werden können. Zum Beispiel könnte die Kennzahl *Umsatz* mit der Formel *Absatz * Preis* berechnet werden. Diese Formeln können die Schlüssel anderer Kennzahlen verwenden, um Berechnungen durchzuführen.  
[Qvantum Wissensdatenbank, Formelmanager](https://lp.qvantum-plan.de/wissensdatenbank/segmente-und-formeln)


 


**Kennzahlenformel**  
Eine Kennzahlenformel ist eine mathematische oder logische Berechnung, die auf einer oder mehreren Kennzahlen basiert. Diese Formeln erlauben es, komplexe Kalkulationen durchzuführen, wie z. B. *Umsatz = Absatz * Preis*.  
[Qvantum Wissensdatenbank, Formelmanager](https://lp.qvantum-plan.de/wissensdatenbank/segmente-und-formeln)


 


**Knoten**  
Ein Knoten ist ein Element innerhalb einer Hierarchie, das andere Elemente oder Detailstufen zusammenfasst. Ein Beispiel wäre eine regionale Vertriebsgruppe, die mehrere lokale Vertriebsstellen als untergeordnete Knoten hat.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-f%C3%BCr-planer)


 


**Konsolidierung**  
Konsolidierung ist der Prozess der Zusammenführung von Daten über mehrere Dimensionen oder Ebenen hinweg. In Qvantum könnte dies bedeuten, dass Daten aus verschiedenen Kostenstellen oder Szenarien in einem Bericht zusammengeführt werden.


**Modellvorlage**  
Die Modellvorlage ist das strukturelle Grundgerüst des Qvantum-Datencubes. Sie enthält alle Dimensionen und Elemente, die in den Planungsprozessen verwendet werden. Benutzer können in der Modellvorlage neue Dimensionen hinzufügen oder bestehende Elemente ändern, um das Modell den spezifischen Anforderungen anzupassen.  
[Qvantum Wissensdatenbank, Modellvorlage](https://lp.qvantum-plan.de/wissensdatenbank/modell)


 


**Owner**  
Der Owner ist eine Rolle, die in Qvantum die Funktion eines Administrators übernimmt. Der Owner ist für die Einrichtung und Pflege der Formulare verantwortlich, die den Planern zur Verfügung gestellt werden. Der Owner legt auch die Berechtigungen fest, die bestimmen, welche Planer auf welche Formulare und Teilwürfel zugreifen dürfen.  

 


**Planer**  
Ein Planer ist ein Benutzer, der in Qvantum Planungsdaten eingibt und bearbeitet. Der Zugriff des Planers ist auf die Formulare und Teilwürfel beschränkt, die ihm zugewiesen wurden. Planer haben in der Regel keine Berechtigung, das Modell zu ändern, sondern können nur auf die ihnen zugewiesenen Daten zugreifen und diese bearbeiten.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-f%C3%BCr-planer)


 


**Referenzspalte/-zeile**  
Bei der Formularbearbeitung in Qvantum kann der Benutzer zur Eingabe eines Wertes auf einem Knoten nach einer Referenzspalte oder -zeile gefragt werden. Wählt der Benutzer eine Referenz, wird der eingetragene Wert nach den gleichen Proportionen verteilt, wie die Verteilung in der Referenzspalte oder -zeile.  
[Qvantum Wissensdatenbank, Referenzspalte/-zeile](https://lp.qvantum-plan.de/wissensdatenbank/verteilm%C3%B6glichkeiten-in-verschachtelten-ebenen)


 


**Segment**  
In Qvantum kann der Datenwürfel entlang einer Dimension wie *Jahre* geschnitten werden, um separate Teilwürfel, sogenannte Segmente, zu erstellen. Ein Segment kann beispielsweise die Daten für die Jahre 2024, 2025 und 2026 jeweils separat darstellen. Der Begriff "Segment" wird in Qvantum synonym für "Teilwürfel" verwendet.  
[Qvantum Wissensdatenbank, Modellvorlage](https://lp.qvantum-plan.de/wissensdatenbank/segmente-und-formeln)


 


**SSO (Single Sign-On)**  
Single Sign-On (SSO) wird in großen Unternehmen häufig als Sicherheitsstandard eingesetzt, da es den Zugriff auf mehrere Anwendungen mit nur einer Authentifizierung ermöglicht. Dies verbessert die Sicherheit, da Benutzer nur ein starkes Passwort für alle Anwendungen benötigen, was das Risiko verringert. Qvantum kann als eine dieser Anwendungen integriert werden, sodass Benutzer nach der einmaligen Anmeldung auf alle verknüpften Systeme zugreifen können.


**Systemeinstellungen**  
Systemeinstellungen in Qvantum ermöglichen es dem Owner, zentrale Konfigurationen für die gesamte Planungsumgebung vorzunehmen. Dazu gehören unter anderem die Verwaltung von Wertetypen, Formatierungen und weiteren Einstellungen, die das Verhalten der Software beeinflussen.


[Systemeinstellungen in Qvantum](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-einstellungen)​


 


**Token**  
Ein Token ist ein digitales Authentifizierungsinstrument, das nach erfolgreicher Anmeldung verwendet wird, um den Zugriff auf bestimmte Daten oder Systeme zu gewähren. Es fungiert als Sicherheitsschlüssel in Netzwerken oder bei API-Zugriffen.


 


**Verteilung im Würfel**  
Verteilung im Würfel bezieht sich auf die automatische Verteilung von Werten entlang einer Dimension. Zum Beispiel könnte ein eingegebener Jahreswert automatisch auf die Monate verteilt werden, wenn die Zeitdimension diese Funktion unterstützt.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-f%C3%BCr-planer)


 


**Wertetypen**  
Wertetypen in Qvantum bestimmen, wie bestimmte Kennzahlen dargestellt und behandelt werden. Es gibt verschiedene Typen wie *Betrag*, *Prozentsatz*, *Preis*, *Menge* und *Bestand*. Diese Wertetypen definieren das Format und die Währungseinheit, in der die Kennzahlen dargestellt werden.  
[Qvantum Wissensdatenbank, Benutzereinstellungen](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-einstellungen)


 


**Workflow zur Planung**  
In Qvantum gibt es drei Stufen im Planungs-Workflow: "Offen" (nachdem die Planung gestartet ist), "Eingereicht" (sobald ein Planer seine Arbeit eingereicht hat), und "Abgenommen" (sobald der Owner die Zahlen abgenommen hat). Dieser Workflow sorgt für einen klaren Ablauf der Planungsphasen.  
[Qvantum Wissensdatenbank, Qvantum für Planer](https://lp.qvantum-plan.de/wissensdatenbank/qvantum-f%C3%BCr-planer)


 


**Zahlformatierungen**  
Zahlformatierungen in Qvantum hängen von den Spracheinstellungen ab. Zum Beispiel wird in der deutschen Einstellung das Format "1.000,00 €" verwendet, während in der englischen Spracheinstellung "1,000.00 €" üblich ist. Dies ist besonders bei der Darstellung von Finanzdaten wichtig.  
[Qvantum Wissensdatenbank, Benutzereinstellungen](https://lp.qvantum-plan.de/wissensdatenbank/zahlformatierungen)


 


**Zellfunktionen**  
Zellen in Qvantum-Formularen können bestimmte Funktionen ausführen, wie z. B. Summenberechnungen oder Verknüpfungen mit anderen Feldern im Formular. Diese automatisierten Funktionen unterstützen eine effiziente Dateneingabe und -bearbeitung.  
[Qvantum Wissensdatenbank, Arbeiten mit Formularen](https://lp.qvantum-plan.de/wissensdatenbank/zellfunktionen)


#### 




**Category:** Modell
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/glossar-begriffe-rund-um-den-datencube)
