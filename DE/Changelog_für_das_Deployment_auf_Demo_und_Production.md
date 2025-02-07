# Changelog für das Deployment auf Demo und Production

**Betrifft: Alle Demo- und Production-Accounts**


### **Changelog für das Deployment auf Demo und Production am 31.01.2024**


* Wertetypen für Berechnete Spalten: Berechneten Spalten, im Kontext manuell konfigurierter Achsen, kann der Controller nun berechneten Spalten/Zeilen einen Wertetyp zuweisen und darüber die Anzeige von Einheiten und Dezimaltrennzeichen steuern.


### **Changelog für das Deployment auf Demo und Production am 23.01.2024**


* In der oberen Menüleiste in QVANTUM gibt es jetzt ein Fragezeichen-Icon, welches direkt mit der Wissensdatenbank verlinkt ist. Der Anwender kann darüber - abhängig von der Stelle, an der er sich in QVANTUM befindet - direkt zur passenden Dokumentation springen.
* Beim Anlegen eines neuen Trial-Tenants steht jetzt auch das GuV-Modell zur Auswahl.


### **Changelog für das Deployment auf Demo und Production am 19.12.2023**


* Der Leere-Zeilen Filter am Formular ist jetzt permanent verfügbar
* Der Fehler, der bei großen Formularen manchmal zur Meldung "Maximum Call stack exceeded" geführt hat, wurde behoben
* Die API wurde um die Möglichkeit, zur Abfrage einer Struktur CSV erweitert


### **Changelog für das Deployment auf Demo und Production am 07.11.2023**


* Formulare und die Einträge im Hauptmenü können jetzt im neuen Tab geöffnet werden.


### **Changelog für das Deployment auf Demo und Production am 09.10.2023**


**Excel Modellvorlage** kann jetzt **komplett auf englisch** geführt werden
* **Download des Modells mit englischer Benutzersprache** erzeugt durchgängig englischsprachiges Modell (Spaltenüberschriften u.a. Teile wurde bis dahin noch auf deutsch geführt)
	+ Modell hat jetzt eine **Spracheinstellung**, die auf dem ersten Tab unter der Versionsnummer platziert ist. Bisher werden allerdings nur **DE** und **EN** unterstützt.
* Beim **Upload des Modells** werden jetzt auch die englischen Spaltenüberschriften interpretiert.



### **Changelog für das Deployment auf Demo und Production am 27.09.2023**


* Demo:
	+ Vorarbeiten für den Formelmanager: Kennzahlen und Formeln sind jetzt auf dem Modelltab einsehbar (Formeln sind noch nicht editierbar)
* Production:
	+ Berechtigungsconstraint bzgl. Ebenenverschachtelung wurde gelockert.


### **Changelog für das Deployment auf Demo und Production am 06.09.2023**


* Neues Feature Ebenenverschachtelung
* Diverse Bugfixes


### **Changelog für das Deployment auf Demo und Production am 27.06.2023**



* Es gibt jetzt ein Dezimalkomma statt einem Dezimalpunkt
* Es gibt neue Zellfunktionen, DIV und MUL



### **Changelog für das Deployment auf Demo und Production am 13.06.2023**



* Diverse Upgrades verwendeter Komponenten
* Modellvorlagen für Standardmodelle ("Modellvorlage herunterladen" auf dem Modell-Tab) wurden überarbeitet und stehen jetzt in neuem Design zur Verfügung
* Das neue Feature ["Changelog"](https://lp.qvantum-plan.de/wissensdatenbank/tab-daten#changelog) kann jetzt pro Tenant (wenn benötigt) aktiviert werden, um Änderungen an den Daten nachzuverfolgen.



### **Changelog für das Deployment auf Demo und Production am 02.05.2023**


Mit diesem Deployment wurden verschiedene Bugs gefixt.
### **Changelog für das Deployment auf Demo und Production am 04.04.2023**



* Spaltenbreiten im Formular speichern
* Englisch-sprachige Modellvorlage zum Download
* Letzte Improvements zu Navigation fixieren/pinnen (graue Box wurde ersetzt)
* Letzte Improvements zu Formatierung von Zeilen/Spalten (neues Icon für Formatierung löschen)
* Kleinere Bugfixes bzgl. Formatierung & Blattverschachtelung



### **Changelog für das Deployment auf Demo und Production am 16.03.2023**



* Leere Ordner werden für Planer nicht mehr angezeigt


Folgende Features nun auf allen Umgebungen aktiv:
* Formatierung von Zeilen und Spalten in den Achsentypen: Dimensionstreu, Blattverschachtelt und Benutzerdefiniert normal. Außerdem für Merkmalspalten.
* Blattverschachtelung wurde grundlegend redesigned, es ist nun (wieder) möglich Teile auf- und zuzuklappen. Das wird auch gespeichert.


Formal nicht dabei, aber schon sichtbar ist außerdem:
* Wenn man QVANTUM auf Englisch benutzt bekommt man eine andere Modellvorlage.



### **Changelog für das Deployment auf Demo und Production am 14.03.2023**



* Trial Umgebung: SSSU nur in dieser Umgebung
* Verschachtelung:
	+ Blattverschachtelung inkl. Aufklappstatus speichern (FT noch aus!)
	+ Ebenenbezeichnungen importieren/exportieren inkl. neue Modellvorlagen für SSSU
* Moduswechsel für Planer unterbinden (vorher Achsenkonfiguration fixieren)
* Cut-Off: komplett ausgebaut
* Bugfixes:
	+ Nutzersynchronisation
	+ Fehlerhaftes/unvollständiges Rechnen nach Modellupdate



### **Changelog für das Deployment auf Demo und Production am 09.02.2023**








* **Performance Optimierungen:**
	+ Zeit für das Modellupdate konnte um ca. 50% verringert werden
	+ Performance beim Speichern von Eingaben im Frontend konnte durch verschiedene Optimierungsmaßnahmen erheblich verbessert werden
* Die **Verschmelzung von Aspekt und Struktur** konnte abgeschlossen werden. Das vereinfacht zukünftige Weiterentwicklungen.
* **Suchfunktion in Dimensionen:** Mehrfache Treffer können jetzt nacheinander aufgerufen werden







### **Changelog für das Deployment auf Demo und Production am 22.12.2022**




Folgende Inhalte wurden live gestellt:


* [**Navigation fixieren, erzwingen, pinnen:**](https://lp.qvantum-plan.de/wissensdatenbank/formulare-für-den-planer-fixieren) der Controller kann die Navigation für den Planer einschränken und die Darstellung in den Formularen auf das Wesentliche reduzieren.
* **Internationalisierung:** die Qvantum App, sowie unsere Webseite, inkl. der Anmeldung über das Self-Service Signup Formular bis hin zu einer englischen Trial Version sind ab jetzt auf Englisch verfügbar. Kleinere Korrekturen folgen noch.
* Kleinere Anpassungen an der Qvantum App:
	+ Der **Kontrast** zwischen Schrift- und Hintergrundfarbe markierte Zeilen oder Spalten wurde für eine bessere Lesbarkeit erhöht.
	+ Beim Login wurden bisher die E-Mailadressen auf **Groß-/Kleinschreibung geprüft**. Das ist nach den internationalen Richtlinien auch korrekt. An dieser Stelle wird aber jetzt für den User eine entsprechende Fehlermeldung angezeigt.
* Die **Konsistenz** der Anwendungsdatenbanken wurde verbessert.



### **Changelog für das Deployment auf Demo und Production am 14.12.2022**


Gemäß unserer Roadmap wurden bereits große Teile des Projekts **„Fixieren, Erzwingen und Pinnen der Navigation“** umgesetzt. Die Funktionen im Einzelnen:


  

* 
	+ In Formularen kann der Controller jetzt Dimensionen, die nicht in den Zeilen oder Spalten liegen fixieren. Hierzu wählt er im Formularkopf einen Knoten aus und fixiert ihn über das Schloss Symbol. Der Planer sieht anstelle des Dropdowns für die Auswahl jetzt den fixierten Knotenpunkt, der mit einem Schloss versehen wurde.
	+ Die Auswahl von Elementen in einer Dimension, die in den Zeilen oder Spalten liegt, kann jetzt nicht mehr über den Formularkopf geändert werden. Die Einstellung kann aber weiterhin über den Zeilen-/Spaltendialog getroffen werden.
	+ In Dimensionen, in denen bisher auf der obersten Ebene mehr als ein Knoten saß, wurde automatisch ein synthetischer Knoten "Alle" angezeigt. Hier hat sich nun die Darstellung geändert, um "Alle" nicht wie einen Knotenpunkt in der Struktur aussehen zu lassen.
	+ Wenn ein Planer keine Berechtigungen auf dem fixierten Element hat ist das Formular für ihn ungültig und wird ausgeblendet.


### **Changelog für das Deployment auf Demo und Production am 22.11.2022**


* Highlights



	+ Weitere Schritte für Internationalisierung
	+ Suchfunktion für Elemente in Dimensionen
	+ Erhöhung der Modellierungsmächtigkeit mit Wald-Strukturen




### **Changelog für das Deployment auf Demo und Production am 25.10.2022**


* Highlights
	+ Redesign Werkzeugleiste
	+ Viele Schritte für Internationalisierung


* 
	+ Ein Bug bei der Backendverteilung wurde gefixt


### **Changelog für das Deployment auf Demo und Production am 12.10.2022**


* Die zweite Verschachtelung (Blätter mit Blättern) ist aktiv


### **Changelog für das Deployment auf Demo und Production am 10.10.2022**


* Bugfixes


### **Changelog für das Deployment auf Demo und Production am 13.09.2022**


* Bugfixes


### **Changelog für das Deployment auf Demo und Production am 05.09.2022**


* Bugfixes bei Bearbeiten und Löschen von Formularen


### **Changelog für das Deployment auf Demo und Production am 23.08.2022**


* Features:
	+ Self-Service Sign-Up inklusive (vorläufiger) Modelle
	+ Performanceverbesserungen (Datenupload + Anfrage)
	+ Ganze Zeile/Spalte markieren (aller erster Schritt von "Formatierung für Grid Zellen")
	+ kleine Bugfixes


### **Changelog für das Deployment auf Demo und Production am 09.06.2022**



* Features:
	+ Formeln: weitere Funktionen, Operatoren & Konstanten
		- Funktionen QUOTIENT & MODULO
		- Funktionen MIN & MAX
		- Boolesche Funktionen ISBLANK & ISVALID
		- Boolesche Operatoren NOT, AND, OR
		- Konstante BLANK
* Bugfixes:
	+ Fehlerhaftes Rechnen im Kontext von Zeitversatz-Formeln



### **Changelog für das Deployment auf Demo und Production am 05.04.2022**



* DIVIDE und SIGN Funktion
* IF Funktion und damit auch Vergleiche, z. B. IF([A] < [2]; [B]; [C] + 1)
* Formulare ohne Berechtigung auf Elemente (z. B. Vertriebseinheiten) werden ausgeblendet.
* Grundzüge der Verschachtelung
* Aktive Zeile/Spalte hervorheben
* Freigabe von Formularen für alle oder keinen oder bestimmte Planer



### **Changelog für das Deployment auf Demo und Production am 04.05.2022**



* Features:
	+ **Bedingungen in Formeln**: Die Formel-Funktion if/wenn ist in Formular- und Kennzahlen-Formeln verfügbar.
	+ **Berechtigungen auf Formularen:** Formulare können für Owner/für alle Planer berechtigt werden. Ein Formular wird für einen Planer automatisch ausgeblendet, wenn der Planer keine Berechtigungen auf allen Elementen der Formular Zeilen- oder Spaltendefinition besitzt.



*  Bugfixes:
	+ **Highlighting Spalten/Zeilenheader:** das Highlighting der Spalten/Zeilenheader bzgl. einer fokussierten Datenzelle im Formular hatte ein fehlerhaftes Verhalten nach Scroll Operationen in größeren Formularen. Mit diesem Bugfix wurde dies korrigiert.
	+ **Formular speichern:** nach dem Speichern einer Änderung an einem Formular wurde die Änderung nach einem Formularwechsel nicht mehr angezeigt, nur nach einem Page Reload. Mit diesem Bugfix werden die Änderungen wieder ohne Page Reload korrekt angezeigt.








### **Changelog für das Deployment auf Demo und Production am 05.04.2022**



In diesem Changelog sind zusätzlich einige Punkte aufgeführt, die bereits seit einiger Zeit deployt sind, aber noch in keinem Changelog erwähnt wurden.

* Features:
	+ Formularordner: Formulare können in Ordnern strukturiert werden.
	+ Ausblenden von leeren Zeilen/Spalten: Formularzeilen/-spalten, die entweder komplett leer oder nur mit 0-Werten befüllt sind, können über einen Filter ein- und ausgeblendet werden.
	+ Admin SSO: Zusätzlich zum SSO für Planer ist SSO auch für Admins von QVANTUM Planungsanwendungen verfügbar.
	+ Navigationslinks auf Formulare: Links auf Formulare können zusätzliche Navigationsinformationen zum Steuern der eingestellten Kopfdimensionen enthalten
	+ Erweiterung Eingabefähigkeit: durch verbesserte Erkennung unabhängiger Würfelbereiche können nun deutlich mehr Würfelzellen in benutzerdefinierten Spalten eingegeben werden, die vorher gesperrt waren. Z.B. war die Spalte IST/Gesamtjahr in Kombination mit PLAN/Januar gesperrt, obwohl beide Spalten in disjunkten Teilwürfeln angesiedelt waren.
	+ Subset Filter in Datenexport API: für Datenanfragen über die Datenexport API können nun Subset Filter über mehrere Dimensionselemente pro Dimension formuliert werden. Damit werden gezieltere Exporte bestimmter Würfelbereiche möglich.






* Bugfixes: Fehler in Backend-Aggregation beseitigt





### **Changelog für das Deployment auf Demo und Production am 19.01.2022**


  

* INFO: Das Formelwerk wurde im Hintergrund für weitere Funktionen vorbereitet. Dadurch haben sich bereits bestehende Formeln evtl. verändert, damit diese das gleiche Verhalten wie vorher zeigen.
* Es wurde ein Fehler behoben, der die Verwendung des Dimensionsblatts „#Dimension“ in der Modellvorlage verhindert hat.
* Es wurden kleinere grafische Fehler auf dem Team-Tab behoben.  
  





---


### Changelog für das Deployment auf Demo und Production am 20.12.2021


* Das Feature „Benutzerdefinierte Zeilen“ wurde weiter verfeinert:
	+ Es ist nun als Owner möglich, benutzerdefinierte Zeilen sofort in den Zeilen zu definieren.
* Es ist nun als Owner möglich, in berechneten Zeilen oder Spalten negative Werte farblich hervorzuheben zu lassen. Diese Einstellung betrifft alle Owner und Editors, die dieses Formular benutzen.
* Im Team-Tab wird nun zwischen den Nutzer-Stammdaten und den Nutzer-Berechtigungen unterschieden.
	+ Es ist nun nötig, Stammdaten und Berechtigungen separat hochzuladen. Mehr Informationen finden Sie hier: [Das Team-Tab](https://lp.qvantum-plan.de/wissensdatenbank/tab-team) und [Nutzer-Berechtigungen](https://lp.qvantum-plan.de/wissensdatenbank/nutzer-berechtigungen-in-qvantum-definieren) in QVANTUM vergeben.


### Changelog für das Deployment auf Demo und Production am 10.11.2021


* Das Feature „Benutzerdefinierte Zeilen“ wurde weiter verfeinert:
	+ Zellen von benutzerdefinierten Zeilen sind nun eingabefähig, wenn sie es als benutzerdefinierte Spalten auch wären.
	+ Berechnete Zellen mit Formeln werden nun nicht nur in den Spalten, sondern auch in den Zeilen angezeigt.
* Bugfixes rund um den neuen Grid-Editor und die neuen benutzerdefinierten Zeilen


### Changelog für das Deployment auf Demo und Production am 25.10.2021


* Neue Features in QVANTUM:
	+ Angelegte benutzerdefinierte Spalten können innerhalb des Formulars zu verschoben werden.
	+ Benutzerdefinierte Spalten können nun in die Zeilen getauscht werden, um benutzerdefinierte Zeilen zu erzeugen.
	+ Formulardefinitionen können nun per API exportiert und importiert werden
* Es wurde ein Fehler behoben, in dem exportierte Modelle mit mehr Spalten exportiert wurden


### Changelog für das Deployment auf Demo und Production am 13.10.2021


* FEATURE: Neuer Formular Editor für schnellere und komfortablere Erstellung von Formularen in QVANTUM
	+ Es ist nun über die Dimensionsanzeige in Formularen möglich, mehr als eine Dimension in die Spalten zu legen.
	+ Fügen Sie einzelne Daten- oder Berechnungsspalten einfach direkt im Formular hinzu, indem Sie auf „+ Spalten hinzufügen“ bzw. „+“ in den Spalten klicken.
	+ Sie können zudem Spalten direkt im Formular bearbeiten oder löschen.
	+ Auch der Spalten-Typ kann nun ohne Löschen der Spalte verändert werden.
	+ Aufgeräumtes, platzsparendes Design.
* Der bisherige Spalten-Editor ist damit obsolet und entfällt.


Mehr Infos, wie Sie den neuen Formular-Editor nutzen können, erfahren Sie in unserem Artikel [Formulare anlegen](https://lp.qvantum-plan.de/wissensdatenbank/formulare-anlegen).


### Changelog für das Deployment auf Demo und Production am 05.10.2021


* CHANGE: Die Art und Weise, wie Berechtigungen auf Elementen deklariert wird, wurde verändert:
	+ Elemente müssen nun in eckige Klammern gesetzt werden
	+ Für Berechtigung auf allen Elementen einer Dimension (ausgenommen Planungseinheiten-Dimension) ist das Keyword ALLE/ALL nutzbar
	+ Alte CSV-Dateien, die noch die Spalte „planning-unit“ enthalten, sind nicht mehr kompatibel und müssen angepasst werden.
* Details finden Sie [im entsprechenden Guide](https://lp.qvantum-plan.de/wissensdatenbank/guide-nutzerberechtigungen-vergeben).


### Changelog für das Deployment auf Demo und Production am 14.09.2021


* FEATURE: Neue Möglichkeit in Formularen, Zeilen- und Spalten anzupassen.
* FEATURE: Neue und genauere Fehlerbehandlung für Modell-, Daten- und Team-Uploads.
* BUGFIX: Es wurde ein Fehler korrigiert, bei dem Formulardefinitionen in der falschen Reihenfolge exportiert und importiert wurden.
* BUGFIX: Es wurde ein Fehler korrigiert, bei dem Merkmale in Formularen nicht bearbeitet werden konnten.
* Kleinere Verbesserungen unter der Haube von QVANTUM.


### Changelog für das Deployment auf Demo und Production am 13.08.2021


* FEATURE: Es ist nun für Controller möglich, [Formulardefinitionen zu exportieren und zu importieren](https://lp.qvantum-plan.de/wissensdatenbank/formulardefinitionen-exportieren-und-importieren).
* FEATURE: Für unterschiedliche Wertetypen werden nun folgende Formatierungen verwendet:
	+ Preis: xx,yy €
	+ Betrag: xx,yy €
	+ Menge: xx,yy
	+ Bestand: xx,yy
	+ Prozent: xx,yy %
* Improvement: Die Darstellung des Dropdown-Menüs bei der Dimensionsnavigation wurde verbessert.
* Improvement: Sollte eine Verarbeitung im Backend länger als 30 Sekunden dauern, wird ein Hinweis angezeigt.
* Kleinere Optimierungen und Bugfixes innerhalb der Software


### Changelog für das Deployment auf Demo und Production am 05.08.2021


* Die Funktion „Zeitversatz“ ist jetzt für Kennzahlenformeln verfügbar.
* Es ist nun möglich, Formulardefinitionen zu exportieren. Der Import dieser Definitionen wird in ca. 2 Wochen verfügbar sein.
* Fehler bei der Berechnung innerer Formeln wurden behoben
* Verbesserte Fehlerbehandlung bei Kennzahlenformeln
* Kleinere Performance-Optimierungen für Planer


Das nächste geplante Update findet voraussichtlich am **17.08.2021** statt.


### Changelog für das Deployment auf Demo und Production am 21.07.2021


* Es ist nun möglich, Berechtigungen auf mehr als nur die „Planungseinheiten“-Dimension zu legen.
* Die Bedienung der Formulare wurde näher an Microsoft Excel angepasst:
	+ Das Standardverhalten beim Anklicken und Doppelklicken von Zellen wurde so verändert, wie es aus Excel gewohnt ist.
	+ Es ist nun einfacher möglich, Bereiche im Formular zu markieren, in sie hineinzukopieren oder den Inhalt herauszukopieren.
	+ Es ist nun möglich, Bereiche im Formular zu löschen.


**Category:** Changelogs
**Keywords:** Changelog,Demo,Production,Updates
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/changelog)
