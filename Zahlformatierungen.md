# Zahlformatierungen

**Sie erhalten eine Übersicht welche Zahlformatierungen in der Anwendung möglich sind. **

### 



Beachten Sie, dass sich Dezimaltrennzeichen und Tausendertrennzeichen von der **Spracheinstellung** ableiten.


Englische Spracheinstellung: 1,000.00€


Deutsche Spracheinstellung: 1.000,00€



### Punkte als Tausendertrennzeichen


Punkte können grundsätzlich als Tausendertrennzeichen verwendet werden. Die falsche Platzierung von Tausendertrennzeichen führt allerdings zu einer Fehlermeldung.:


[![zahlenformatierung_trennzeichen-1](https://lp.qvantum-plan.de/hubfs/zahlenformatierung_trennzeichen-1.png)](https://lp.qvantum-plan.de/hubfs/zahlenformatierung_trennzeichen-1.png)


 


Richtig wären die Schreibweisen 1.000 oder 1.000,00.


[![zahlformatierung_trennzeichen2-1](https://lp.qvantum-plan.de/hubfs/zahlformatierung_trennzeichen2-1.png)](https://lp.qvantum-plan.de/hubfs/zahlformatierung_trennzeichen2-1.png)


### Komma als Dezimaltrennzeichen


Es darf maximal ein Komma als Dezimaltrennzeichen verwendet werden. Vor und hinter dem Komma muss sich mindestens eine Ziffer befinden.


Falsche Eingabe:


[![zahlformatierung_dezimaltrennzeichen](https://lp.qvantum-plan.de/hubfs/zahlformatierung_dezimaltrennzeichen.png)](https://lp.qvantum-plan.de/hubfs/zahlformatierung_dezimaltrennzeichen.png)


Richtig:


[![zahlformatierung_dezimaltrennzeichen2](https://lp.qvantum-plan.de/hubfs/zahlformatierung_dezimaltrennzeichen2.png)](https://lp.qvantum-plan.de/hubfs/zahlformatierung_dezimaltrennzeichen2.png)


### Zellfunktionen


Zellfunktionen können verwendet werden. Mehr über [Zellfunktionen](https://lp.qvantum-plan.de/wissensdatenbank/zellfunktionen).


### Minuszeichen


Sie dürfen maximal ein vorangestelltes Minus verwenden. 



Ein Minuszeichen darf nicht mit einer [Zellfunktion](https://lp.qvantum-plan.de/wissensdatenbank/zellfunktionen) in derselben Formularzelle verwendet werden.



Fehlermeldung mit zwei Minuszeichen:


[![zahlformatierung_minus](https://lp.qvantum-plan.de/hubfs/zahlformatierung_minus.png)](https://lp.qvantum-plan.de/hubfs/zahlformatierung_minus.png)


Beispiel:


[![zahlformatierung_minus2](https://lp.qvantum-plan.de/hubfs/zahlformatierung_minus2.png)](https://lp.qvantum-plan.de/hubfs/zahlformatierung_minus2.png)


### Formatierung mit Einheiten


Die Zeichenfolge, die zum Wertetyp der zu ändernden Zelle gehört, darf nach der Zahl verwendet werden. Jede Zelle hat genau einen von 5 möglichen Wertetypen. Der Owner kann für jeden dieser Wertetypen eine Zeichenfolge als Einheit definieren.


Beispiel:


Für den Wertetyp "Preis" könnte die Zeichenfolge "EUR" und für den Wertetyp "Prozentsatz" die Zeichenfolge "%" festgelegt worden sein. Dann wäre die Eingabe "3EUR" für eine "Preis"-Zelle erlaubt. Verboten wären für dieselbe Zelle "3€" oder "3$", weil das jeweils nicht die vorgegebene Zeichenfolge ist und auch "3%" ist nicht erlaubt, weil es keine "Prozentsatz"-Zelle ist. Wenn Sie die Zelle verlassen, formatieren wir die Zahl wie vom Owner festgelegt, daran können Sie die korrekte Zeichenfolge ablesen.


Zwischen der Zahl und der Zeichenfolge dürfen beliebig viele Leerzeichen stehen.


Beispiel:


[![zahlformatierung_einheiten](https://lp.qvantum-plan.de/hubfs/zahlformatierung_einheiten.png)](https://lp.qvantum-plan.de/hubfs/zahlformatierung_einheiten.png)


### Multiplizieren von Zahlen mit K oder M


Die Zeichen **K** und **M** dienen als Abkürzungen für **Tausend** und **Millionen**. 


#### Multiplizieren mit Tausend (K)



```
<Zahl>K oder <Zahl>k multipliziert <Zahl> mit 1.000
```

Vorher:


[![Zellfunktion K](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_k-1200x545.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_k-1200x545.png)


Nachher:


[![Zellfunktion K](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_k1-1024x486.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_k1-1024x486.png)


#### Multiplizieren mit Million (M)



```
<Zahl>M oder <Zahl>m multipliziert <Zahl> mit 1.000.000
```

Vorher:


[![Zellfunktion M](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_m-1024x486.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_m-1024x486.png)


Nachher:


[![Zellfunktion M](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_m1.png)](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_m1.png)


 



**Category:** Formulare
**Subcategory:** Arbeiten mit Formularen
**Keywords:** Formatierung,Zahlenformatierung
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/zahlformatierungen)
