# Rechenoperationen und Formelsyntax

**QVANTUM unterstützt die auf dieser Seite definierten Rechenoperationen und Formeln. **

Die hier aufgeführten Rechenoperationen und Formeln lassen sich sowohl im **Formelmanager** ([hier](https://lp.qvantum-plan.de/wissensdatenbank/segmente-und-formeln) finden Sie weitere Hilfe zur Eingabe von Formeln im Formelmanager) als auch in Berechnungsspalten von Formularen verwenden.


### Inhalt dieser Seite


* Allgemeines zur Verwendung von Argumenten in Funktionen
* [Rechenoperationen](#Rechenoperationen)
* [Formeln und Funktionen](#Formeln-und-Funktionen)
* [Vergleichsoperatoren](#Vergleichsoperatoren)


### 



### Allgemeines zur Verwendung von Argumenten in Funktionen


#### Allgemeine Regeln für Kennzahlformeln:


* Für die Argumente einer Funktion werden in der Regel Kennzahlenschlüssel in eckigen Klammern verwendet (z.B. `ABS([DELTA])`). Alternativ können auch Konstanten genutzt werden.


#### Benutzerdefinierte Zeilen- oder Spaltendefinitionen in Formularen:


* In Formularen werden für die Argumente einer Funktion Zeilen- oder Spaltenbezeichner in eckigen Klammern verwendet (z.B. `ABS([3])` oder `ABS([B])`). Auch hier können Konstanten verwendet werden.


#### Kombination von Ausdrücken:


* Formelausdrücke können durch Kombination der oben genannten Angaben und durch Verwendung von Klammerungen gebildet werden (z.B. `ABS(([A]-[B])/[C])`).


#### Funktionsaufrufe innerhalb von Formeln:


* Auch Funktionsaufrufe können in den Formelausdrücken genutzt werden (z.B. `ABS(DIVIDE([1];[2];BLANK))`).


#### Groß-/Kleinschreibung:


* Die Groß- oder Kleinschreibung der Funktionsnamen spielt keine Rolle, sie können beliebig verwendet werden.


#### Besonderheiten bei der Division:


* Bei einer Division durch Null wird der Wert UNGÜLTIG erzeugt, es sei denn, die Funktion `DIVIDE` (siehe unten) wird für die Division genutzt.


#### Leere Zellen:


* Leere Zellen haben den Wert BLANK.


#### Auswertung von Bedingungen:


* Eine ausgewertete Bedingung (siehe `WENN`-Funktion) hat den Wert TRUE, wenn sie erfüllt ist, ansonsten FALSE.


#### Beispiel:


Eine Kennzahl für Erlöse könnte wie folgt definiert werden:



`Erlöse = [VE]*[PPE]`, wobei `VE` der Schlüssel für „Verkaufte Einheiten“ und `PPE` der Schlüssel für „Preis pro Einheit“ ist.


### Rechenoperationen


Addition (+)  
Subtraktion (-)  
Multiplikation (*)  
Division ( / )  
Runde Klammern



 


### Formeln und Funktionen


* [ABS](#abs)
* [COALESCE](#coalesce)
* [DIVIDE](#divide)
* [RUNDEN](#runden)
* [SIGN](#sign)
* [WENN](#wenn)
* [ZEITVERSATZ](#zeitversatz)
* [MODULO](#modulo)
* [QUOTIENT](#quotient)
* [MINIMUM](#Minimum)
* [MAXIMUM](#Maximum)
* [SUMOFCHILDREN](#Sumofchildren)
* [TIMEOFFSET](#timeoffset)
* [ISBLANK](#isblank)
* [ISVALID](#isvalid)
* [AND](#and)
* [OR](#or)
* [NOT](#not)



#### ABS


Gibt den Absolutwert des Arguments zurück. Das bedeutet, dass alle negativen Vorzeichen entfernt werden und der positive Wert zurückgegeben wird. 


Syntax: 



```
ABS(<Wert>) 
```

**Sonderfälle:**


* Betrag von UNGÜLTIG = UNGÜLTIG
* Betrag von BLANK = BLANK



#### COALESCE


Gibt den ersten Ausdruck zurück, der nicht als BLANK ausgewertet wird. Wenn alle Ausdrücke als BLANK ausgewertet werden, wird BLANK zurückgegeben. Die Funktion hat mindestens 2 oder mehr Argumente.


**Syntax:**



```
COALESCE(<Argument1>; <Argument2> [;<Argument3>…])
```


#### DIVIDE


Führt eine Division aus und gibt ein alternatives Ergebnis oder BLANK bei Division durch 0 zurück.


**Syntax:**



```
DIVIDE(<Dividend>; <Divisor> [;<alternatives Resultat])
```

Das alternative Resultat für eine Division durch 0 muss eine Konstante sein. Fehlt die Angabe so ist bei Division durch 0 das Resultat BLANK.


**Sonderfälle:**


* UNGÜLTIG / x und x / UNGÜLTIG ergibt UNGÜLTIG
* BLANK / BLANK ergibt BLANK
* x / BLANK ergibt das alternative Resultat
* x ist eine beliebig gültige Zahl



#### RUNDEN


Rundet eine Zahl auf die angegebene Anzahl von Stellen.


**Syntax:**



```
RUNDEN(<Argument> [; <Anzahl Stellen>])
```

Mit <Argument > bestimmen Sie, welche Zahl gerundet werden soll. Die Anzahl der Stellen ist die Anzahl der Dezimalstellen, auf die Sie runden möchten. Bei einem negativen Wert werden Stellen links vom Dezimaltrennzeichen gerundet. Beim Wert 0 oder wenn die Anzahl der Stellen nicht angegeben wird, wird auf die nächste ganze Zahl gerundet. Die Anzahl Stellen muss eine Konstante sein.



#### SIGN


Gibt das Vorzeichen des gegebenen Wertes zurück. Die Funktion gibt -1, 0 oder 1 zurück, je nachdem, ob der Wert negativ, null oder positiv ist. Dies kann verwendet werden, um schnell das Vorzeichen eines Wertes zu bestimmen. 


Syntax: 



```
SIGN(<Wert>) 
```

**Sonderfälle:**


* Betrag von UNGÜLTIG = UNGÜLTIG
* Betrag von BLANK = BLANK



#### WENN


Prüft eine Bedingung und gibt einen Wert zurück, wenn diese TRUE ist; andernfalls wird ein zweiter Wert zurückgegeben.


**Syntax:**



```
WENN(<Bedingung>;<Wert wenn TRUE>;<Wert wenn FALSE>)
```

<Bedingung> setzt sich zusammen aus einem <Argument1> und einem <Argument2>, die durch einen [Vergleichsoperator](#Vergleichsoperatoren) voneinander getrennt sind.


**Sonderfälle:**  
Sind <Argument1> oder <Argument2> leer, wird das Argument als 0 interpretiert.



#### ZEITVERSATZ


Diese Funktion ermöglicht es, in einer Kennzahlenformel auf ein Vorgängerelement der Zeit-Dimension zuzugreifen.


**Syntax:**



```
ZEITVERSATZ(<Argument>;<Relativer Vorgänger>)
```

Voraussetzung ist die Definition einer Dimension mit der Dimensionsrolle Zeit. Typischerweise sind dies die Monate. Die Funktion wirkt nur auf den Blättern (unterste Ebene) dieser Dimension.


Das <Argument> muss ein Kennzahlschlüssel sein, ein Formelausdruck ist nicht erlaubt. In Formularformeln steht die Funktion nicht zur Verfügung.


Der <Relative Vorgänger> ist eine negative Konstante und bezeichnet die Schrittweite, um das Vorgängerelement ermitteln zu können.


Das Vorgängerelement ist das in der Reihenfolge der Dimensionselemente relativ um die angegebene Schrittweite weiter oben liegende Blatt. Elemente, die keine Blätter sind, werden dabei nicht mitgezählt. Die Funktion wirkt gemäß der Reihenfolge der Dimensionselemente nicht auf dem 1. Blatt, welches aber auch nicht eingabefähig ist. Deshalb muss der Startwert in einer weiteren Kennzahl eingegeben werden. Eine Formel für eine Kennzahl x kann in der ZEITVERSATZ-Funktion ausnahmsweise die Zielkennzahl x auch als Argument verwenden (z.B. im Sinne von [ANZAHL\_KUNDEN] = [KUNDEN\_ZUGANG] + ZEITVERSATZ([ANZAHL\_KUNDEN];-1)).



#### MODULO


Modulo gibt den Rest einer ganzzahligen Division zurück.


**Beispiel:** 


15 mod 12 = 3, da 15 : 12 = 1, 3 bleibt übrig


**Syntax:**



```
MODULO(<Dividend>; <Divisor>)
```

**Beispiel:**


Im folgenden Beispiel wurde die Formel MODULO([B];[A]) verwendet.  


![](https://lp.qvantum-plan.de/hubfs/undefined.png)



#### QUOTIENT


Bildet den Quotient aus Divident und Divisor. Zurückgegeben wird immer eine Ganzzahl.


**Syntax:** 



```
QUOTIENT(<Dividend>; <Divisor>) 
```

**Beispiel:**


QUOTIENT(5;3) 


Das Ergebnis ist 1, da die Nachkommastellen entfallen.



#### MINIMUM


Gibt das Minimum der gegebenen Argumente zurück. 


Syntax: 



```
MINIMUM(<Argument1> [;<Argument2>;<Argument3>…]) 
```


#### MAXIMUM


Gibt das Maximum der gegebenen Argumente zurück. Diese Funktion ermöglicht es, den größten Wert aus einer Liste von Werten zu ermitteln. 


Syntax: 



```
MAXIMUM(<Argument1> [;<Argument2>;<Argument3>…]) 
```


#### SUMOFCHILDREN


Summiert die Werte der Kinder des aktuellen Elements. Dies ist besonders nützlich für hierarchische Berechnungen, bei denen die Gesamtsumme aus den Werten der untergeordneten Elemente ermittelt werden muss. 


Syntax: 



```
SUMOFCHILDREN() 
```


#### TIMEOFFSET


Nimmt den Wert der referenzierten Kennzahl von einem vorhergehenden Element in der Zeitdimension. Dies ermöglicht zeitbasierte Berechnungen, wie z.B. das Vergleichen von Werten über verschiedene Zeiträume hinweg oder auch das Fortschreiben von Werten für Bestände.


Syntax: 



```
TIMEOFFSET(<Kennzahl>; <Offset>) 
```


#### ISBLANK


Prüft, ob das gegebene Argument leer ist. 


Syntax: 



```
ISBLANK(<Argument>) 
```


#### ISVALID


Prüft, ob das gegebene Argument eine gültige Zahl ist. 


Syntax: 



```
ISVALID(<Argument>) 
```


#### AND


Funktionale Version von &&. Diese Funktion ermöglicht es, zwei Bedingungen in einer Funktionsform zu kombinieren. 


Syntax: 



```
AND(<Argument1>; <Argument2>) 
```


#### OR


Funktionale Version von ||. Diese Funktion ermöglicht es, mehrere alternative Bedingungen in einer Funktionsform zu kombinieren. 


Syntax: 



```
OR(<Argument1>; <Argument2>) 
```


#### NOT


Funktionale Version von !. Diese Funktion ermöglicht die Negation einer Bedingung in einer Funktionsform. 


Syntax: 



```
NOT(<Argument>) 
```


### Vergleichsoperatoren


#### >  (Größer als)


Vergleicht zwei Werte und gibt genau dann TRUE zurück, wenn der erste Wert größer als der zweite Wert ist. 


Syntax: 



```
<Wert1> > <Wert2> 
```

#### >=  (Größer oder gleich)


Vergleicht zwei Werte und gibt TRUE zurück, wenn der erste Wert größer oder gleich dem zweiten Wert ist. 


Syntax: 



```
<Wert1> >= <Wert2> 
```

#### <  (Kleiner als)


Vergleicht zwei Werte und gibt TRUE zurück, wenn der erste Wert kleiner als der zweite Wert ist. 


Syntax: 



```
<Wert1> < <Wert2> 
```

#### <=  (Kleiner oder gleich)


Vergleicht zwei Werte und gibt TRUE zurück, wenn der erste Wert kleiner oder gleich dem zweiten Wert ist. 


Syntax: 



```
<Wert1> <= <Wert2> 
```

#### =  (Gleich)


Vergleicht zwei Werte und gibt TRUE zurück, wenn beide Werte gleich sind. 


Syntax: 



```
<Wert1> = <Wert2> 
```

#### !=  (Nicht gleich)


Vergleicht zwei Werte und gibt TRUE zurück, wenn die Werte ungleich sind. 


Syntax: 



```
<Wert1> != <Wert2> 
```

#### <> (Nicht gleich)


Vergleicht zwei Werte und gibt TRUE zurück, wenn die Werte ungleich sind. Dies ist eine alternative Schreibweise für != und erfüllt denselben Zweck. 


Syntax: 



```
<Wert1> <> <Wert2> 
```

#### && (Und)


Logisches UND, gibt TRUE zurück, wenn beide Operanden TRUE sind. Dieser Operator wird verwendet, um zu überprüfen, ob mehrere Bedingungen gleichzeitig erfüllt sind. 


Syntax: 



```
<Bedingung1> && <Bedingung2> 
```

#### ||  (Oder)


Logisches ODER, gibt TRUE zurück, wenn mindestens einer der Operanden TRUE ist. Dies ist hilfreich, um Bedingungen zu formulieren, bei denen mindestens eine von mehreren Bedingungen zutreffen soll. 


Syntax: 



```
<Bedingung1> || <Bedingung2> 
```

#### !  (Logische Negation)


Logische Negation, gibt TRUE zurück, wenn der Operand FALSE ist. Dieser Operator wird verwendet, um die Wahrheit einer Bedingung zu invertieren. 


Syntax: 



```
!<Bedingung> 
```

 



**Category:** Modell
**Subcategory:** Formelmanager
**Keywords:** Formel,Rechenoperationen
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/rechenoperationen)
