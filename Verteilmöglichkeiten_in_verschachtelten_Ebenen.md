# Verteilmöglichkeiten in verschachtelten Ebenen

**Qvantum bietet verschiedene Möglichkeiten, auch auf aggregierte Strukturelemente zu schreiben. Dabei können die eingetragenen Werte nicht nur in einer Dimension auf die Kindelemente verteilt werden. **

### Die Aggregation auf inneren Knoten


Schauen wir uns zunächst an, wie die Elemente innerhalb einer Struktur aggregiert werden.


#### Beispiel Dimension 1: Aggregation in der Dimension „Monate“


Abbildung 1 veranschaulicht das für die Dimension „Monate“. Die einzelnen Elemente der Monate werden zu Quartalen zusammengefasst. Die Quartale selbst werden wieder zum Gesamtjahr aufsummiert.


Das Strukturelement Q1 ist mit der Aggregationsregel „Summe“ belegt. Es enthält demnach immer die Summe seiner Kindelemente (Januar, Februar und März).  
  



![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-01-57-17-0094-PM.png)  
*Abbildung 1 – Die Monate werden zu Quartalen, die Quartale zum Gesamtjahr aufsummiert*


### Beispiel Dimension 2: Aggregation in der Dimension „Organisationseinheit“


Abbildung 2 zeigt, wie sich die einzelnen Elemente (Mitarbeiter) zu dem jeweils darüber liegenden Knoten (Abteilungen) aufsummieren.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-01-57-48-4208-PM.png)  
*Abbildung 2 – Organisationsstruktur: Die Mitarbeiter werden zu Abteilungen und die Abteilungen zur gesamten Organisation aufsummiert*


### Referenzen für die Verteilung


Wird ein Wert auf seine Kindelemente verteilt, kann das durch Angabe einer Referenz (-Spalte oder -Zeile) geschehen.


Abbildung 3 zeigt, wie die Verteilung unter Auswahl einer Referenzspalte/-zeile funktioniert. Wenn ich z.B. den neuen Wert „60“ für Q1 eintrage kann ich als Referenz Q2 auswählen. Damit übernehme ich das Verhältnis der drei Monate untereinander (April, Mai, Juni: 30, 40, 50), nicht aber die Werte! Diese müssen zusammen genau „60“ ergeben und im Verhältnis 3:4:5 stehen. Damit ergeben sich die Werte 15, 20 und 25 als neue Monatswerte für Q1.  
  



![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-01-58-57-0350-PM.png)  
*Abbildung 3 – Verteilung nach Referenzspalte/-zeile*


Nicht immer ist die Auswahl von Referenzen möglich. Werden die drei Monate (Jan, Feb, Mar) nicht im Formular angezeigt, kann ich trotzdem einen neuen Wert für das Quartal eintragen. Die Verteilung erfolgt dann als „Selbstreferenz“. Abbildung 4 verdeutlicht das.  
  




**Verteilung nach Selbstreferenz**


Wenn ein Strukturelement die Werte seiner Kind-Elemente aufsummiert, lässt sich dieser aggregierte Wert nach der Selbstreferenz verteilen. In diesem Fall wird der neue Wert so auf die Kindelemente verteilt, dass sich das Verhältnis seiner Kindelemente untereinander nicht verändert. Abbildung 4 veranschaulicht, wie sich ein auf Q1 eingetragener Wert nach Selbstreferenz verteilt.



 


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-01-59-39-9924-PM.png)


*Abbildung 4 – Verteilung nach Selbstreferenz* 


  

### Wie funktioniert jetzt die Verteilung von Eingaben im Formular?


#### Verteilung in Formularen mit dimensionstreuen Achsen


In Abbildung V1.1 ist ein Formular mit dimensionstreuen Achsen zu sehen. In den Zeilen liegt die Dimension „Organisationseinheiten“ und in den Spalten liegt die Dimension „Monate“. Alle weißen Zellen sind eingabefähig.


Auch zu beachten ist der Formularheader mit der Kennzahl „Basisgehalt“, der Variante „Plan“, dem „Best Case“ Szenario, sowie dem Jahr „2023“.  
  



*![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-00-32-4483-PM.png)**Abbildung V1.1 – Formular mit dimensionstreuen Achsen – Eingabe auf Vertrieb/Januar*


#### 1. Verteilung der Summe für die Abteilung auf die einzelnen Mitarbeiter


Wenn ich den Wert, den die Vertriebsabteilung im Januar 2023 ausmacht, auf 13.000 € erhöhen möchte, fragt Qvantum nach einer Referenzspalte (Abbildung V1.2). Die 13.000 € entsprechen natürlich am Ende der Summe Ihrer Kindelemente (der drei Mitarbeiter). Ich entscheide mich für die Referenzspalte „Januar“ und ändere damit das Verhältnis der Gehälter untereinander **nicht** (siehe Abbildung V1.3).  
  



![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-00-42-4478-PM.png)  
*Abbildung V1.2 – Auswahl einer Referenzspalte für meine Eingabe*


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-00-47-6750-PM.png)  
*Abbildung V1.3 – Die Gehälter der Mitarbeiter wurden neu berechnet, um in der Summe auf die 13.000 € zu kommen*


#### 2. Verteilung der Quartalssumme auf die einzelnen Monate


In diesem Beispiel möchte ich für einen Mitarbeiter 14.000 € auf das Quartal 1 schreiben. Hierfür muss ich nun eine Referenzzeile auswählen.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-01-02-2109-PM.png)


*Abbildung V2.1 – Verteilung der Quartalssumme der monatlichen Basisbezüge für Mitarbeiter Andre* 


Indem ich dieses erhöhte Basisgehalt anhand der Referenzzeile „Gesamtunternehmen“ auf die Monate verteile, nehme ich den Anstieg der firmenweiten Gehälter in Q1 als Referenz für dieses Mitarbeitergehalt.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-01-08-7848-PM.png)


*Abbildung V2.2 – Verteilung anhand der Referenzspalte „Gesamtunternehmen“*


 


Abbildung V2.3 zeigt das Ergebnis der Verteilung . Die Wahl der Referenzspalte hat dazu geführt, dass das Verhältnis der firmenweiten Gehälter für Januar, Februar und März untereinander übernommen wird. Die Summe der Gehälter dieses Mitarbeiters (von Januar – März) muss dabei trotzdem den eingetragenen 14.000 € entsprechen.


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-01-15-9713-PM.png)


*Abbildung V2.3 – Verteilung des Quartalswert auf die einzelnen Monate*


 


### Verteilung in Formularen mit verschachtelten Ebenen


Um einen Eindruck der erweiterten Verteilmöglichkeiten in einem Formular mit verschachtelten Ebenen zu bekommen, eignet sich das nachfolgend abgebildete Formular. In den Zeilen ist lediglich eine einzige Ebene enthalten:


Die Ebene „Abteilungen“ der Dimension „Organisationseinheiten“.


In den Spalten liegen die Ebene „Jahre“ der gleichnamigen Dimension, sowie die Ebene „Quartale“ der Dimension „Monate“.  
  



*![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-01-25-9904-PM.png)**Abbildung V3.1 – Formular im Modus „Automatisch nach Ebenen“*


 


#### 3. Verteilung auf Mitarbeiter und Monate über verschachtelte Ebenen


Für dieses Beispiel verwenden wir wieder die Dimensionen „Organisationseinheiten“ und „Monate“, deren Strukturen in Abbildungen 1 und 2 dargestellt sind. Allerdings verwenden wir in diesem Formular aus der Dimension „Organisationseinheiten“ nur die Ebene „Abteilungen“ und zeigen die Ebene „Mitarbeiter“ nicht an. Genauso werden die Quartale angezeigt, die Monate aber nicht.  
  



*![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-01-35-0532-PM.png)**Abbildung V3.2 – Eingabe auf Quartals- und Abteilungsebene*


Wenn ich jetzt die Bezüge für die Abteilung „Vertrieb“ in Q1 auf 43.000 € anhebe, kann ich diesen Wert einfach durch Drücken der Enter-Taste übernehmen. Im Formular ist von einer Verteilung nichts zu sehen. Das liegt daran, dass alle Elemente, auf die meine Eingabe verteilt wird, nicht im Formular liegen. Insofern kann ich auch keine Referenzzeile oder -spalte angeben . Die Verteilung erfolgt nach Selbstreferenz.


#### 4. Mehrdimensionale Verteilung in den Zeilen


Das nachfolgende Beispiel (siehe auch Abbildung V4.1) ist nur über den Modus „Automatisch nach Ebenen“ möglich und orientiert sich an den gleichen Beispielstrukturen, die auch in den anderen Beispielen verwendet werden.


Die Zeilen enthalten hier lediglich die Ebene „Abteilungen“ (aus der Dimension „Organisationseinheiten“) und die Ebene „Quartale“ aus der Zeitdimension „Monate“. Abbildung V4.2 zeigt, wie die Achse für dieses Beispiel konfiguriert wurde.


Mit dem Eintragen eines Wertes für Q1/2022 wird die folgende Verteilung angestoßen:


* Der eingetragene Wert muss der Summe der Monate Januar, Februar und März entsprechen. Die Werte für Januar, Februar und März werden neu berechnet. Dabei gilt:
	+ Das Vertriebsgehalt der drei Monate muss im gleichen Verhältnis stehen, wie es auch aktuell der Fall ist (Selbstreferenz).
		- Beispiel: Das Vertriebsgehalt (Summe der Gehälter aller drei Mitarbeiter) ist in den drei Monaten identisch. Damit wäre in jedem der drei Monate der Wert 10.816,67 eingetragen. Ein neu eingetragener Wert würde demnach einfach durch drei geteilt.
	+ Der eingetragene Wert muss der Summe der einzelnen Bezüge aller drei Mitarbeiter des Vertriebs entsprechen. Die Gehälter werden neu berechnet:
		- Die Quartalsgehälter der drei Mitarbeiter müssen im gleichen Verhältnis stehen, wie es aktuell der Fall ist (Selbstreferenz).


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-01-47-5039-PM.png)


*Abbildung V4.1 – Mehrdimensionale Verteilung auf Monate und Mitarbeiter*


 


![](https://lp.qvantum-plan.de/hubfs/image-png-Sep-20-2023-02-01-53-8740-PM.png)  
*Abbildung V4.2 – Konfiguration für die mehrdimensionale Verteilung aus Abbildung V4.1*



**Category:** Formulare
**Subcategory:** Arbeiten mit Formularen
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/verteilmöglichkeiten-in-verschachtelten-ebenen)
