# Changelog für das Deployment auf Demo und Production 2021

**Betrifft: Alle Demo- und Production-Accounts**

### test


Einfach und schnell das perfekte Formular erstellen.


Das neue Feature zur "Verschachtelung von Ebenen" bietet nicht nur eine verbesserte Übersichtlichkeit und Effizienz bei der Eingabe von Plandaten, sondern eröffnet auch ganz neue Möglichkeiten bei der Analyse. Mit dem flexiblen Formularaufbau können Sie Ihre Daten schnell aus verschiedenen Perspektiven betrachten und völlig neue Erkenntnisse gewinnen.


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


**Keywords:** Changelog,Demo,Production,Updates
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/changelog/2021)
