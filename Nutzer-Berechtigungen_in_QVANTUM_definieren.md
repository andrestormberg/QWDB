# Nutzer-Berechtigungen in QVANTUM definieren

**Über den CSV-Upload Berechtigungen definieren**

Über den Berechtigungs-Upload im CSV-Format können Sie die Berechtigungen Ihres gesamten Teams auf einmal anpassen. Voraussetzung ist, dass Sie bereits [Team-Stammdaten importiert](https://lp.qvantum-plan.de/wissensdatenbank/tab-team) haben.  
  
Im Berechtigungs-CSV gibt drei „Basisspalten“, die immer gesetzt werden müssen.





| **email** | **[Dimensionsname]** | **input** |



Für die Berechtigungen sind die Spalte „[Dimensionsname]“ und „input“ relevant.



Hinweis: Alle Nutzer, die nicht explizit im Berechtigungs-CSV aufgeführt werden, verlieren nach dem Import alle bisher vorhandenen Berechtigungen in QVANTUM.



### Spalte „[Dimensionsname]“


Bei dieser Spalte handelt es sich um einen Platzhalter, der mit dem Namen der Dimension mit der Rolle „Planungseinheiten“ gefüllt werden muss. Nutzen Sie den Berechtigungsexport, wird der Name der Dimension automatisch gesetzt.


#### Besonderheiten der Dimension mit der Rolle „Planungseinheiten“


Pro Modell muss es eine Dimension geben, die Rolle „Planungseinheit“ besitzt. Diese definiert die Basis-Berechtigung für die Nutzer, die auch für den Workflow herangezogen wird. Jedem Nutzer muss ein beliebiges Element dieser Dimension zugewiesen werden.  
  
Auch der Wurzelknoten (z. B. „Alle Vertriebseinheiten“) kann als Berechtigung definiert werden, indem Sie entweder das genaue Element berechtigen oder das Schlüsselwort „alle“ oder „all“ (ohne Anführungszeichen oder eckige Klammern) in die betroffene Spalte schreiben.


Beispiel-CSV für Berechtigungen:[![CSV für Berechtigungen](https://lp.qvantum-plan.de/hubfs/Imported%20images/image-7.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/image-7.png)


### Spalte „Input“


Werte ja (Alternativen: yes oder y) geben an, dass die Berechtigung „lesen und schreiben“ gesetzt ist. Die Werte nein (Alternativen: no oder n) geben an, dass ausschließlich die Berechtigung zum Lesen von Werten vorhanden sind.  
  
Die tatsächlichen Berechtigungen werden als eigene Spalte im CSV definiert. Dazu wird der Singular-Name der Dimension als Spaltenüberschrift verwendet, z. B. „Vertriebseinheit“ oder „Produkt“. Als Werte der Spalte werden dann die Schlüssel der Dimensionselemente eingetragen.


### Auf mehreren Elementen einer Dimension berechtigen


Sie können Berechtigungen auch auf mehr als ein Element einer Dimension setzen. Dies kann auf zwei Wegen geschehen:


1. Sie berechtigen einen Nutzer auf einem Element mit hierarchisch untergeordneten Elementen („Knoten“): Der Nutzer ist automatisch auf allen untergeordneten Knoten berechtigt. Geben Sie dazu einfach den Schlüssel des obersten Elements an, auf dem Sie berechtigen möchten.
2. Sie berechtigen einen Nutzer manuell auf mehreren Elementen: Geben Sie in eine Spalte beliebig viele Schlüssel der Dimension an. Einzelne Schlüssel werden durch eckige Klammern voneinander getrennt. Es können einzelne oder hierarchiche Elemente sein. Das Beispiel „[Produkt1] [Produkt2] [Produktgruppe 2]“ in der Spalte „Produkt“ berechtigt auf den einzelnen Produkten 1 und 2 und zusätzlich auf der Produktgruppe 2.


In allen Dimensionen außer der Dimension mit der Rolle „Planungseinheiten“ gilt: Wird ein Wert für einen Nutzer leer gelassen, gilt die Berechtigung automatisch für alle Elemente der Dimension.


 


### Besonderheiten für Formulare mit verschachtelten Ebenen


Formulare mit verschachtelten Ebenen weisen einige Besonderheiten auf. Durch die Verschachtelung einzelner Ebenen unterschiedlicher Dimensionen, können Berechtigungen dem Aufbau einer logischen Struktur im Weg stehen.


Es gelten zwei grundlegende Regeln, damit die Berechtigungen mit den im Formular verwendeten verschachtelten Ebenen kompatibel sind:


* Die Berechtigungen müssen innerhalb einer Dimension auf der gleichen hierarchischen Ebene gesetzt sein.
* Es darf keine Ebene im Formular verwendet werden, auf die der Planer nicht berechtigt ist.


**Category:** Team
**Subcategory:** Nutzer-Berechtigungen
**Keywords:** Berechtigungen,Nutzer,berechti
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/nutzer-berechtigungen-in-qvantum-definieren)
