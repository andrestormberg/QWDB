# Number formatting

**You will get an overview which number formatting options are possible in the application.**

### Dots as a separator for thousand


You can use dots as separators for thousand, but they must appear in the correct place when used.   
  
Error message:


![zahlenformatierung_trennzeichen-1_en](https://lp.qvantum-plan.de/hubfs/zahlenformatierung_trennzeichen-1_en.png)


Correct formatting:


![zahlformatierung_trennzeichen2-1_en](https://lp.qvantum-plan.de/hubfs/zahlformatierung_trennzeichen2-1_en.png)


### Comma as a decimal separator


A maximum of one comma may be used as a decimal separator. There must be at least one digit before and after the comma.  
  
Incorrect input:


![zahlformatierung_dezimaltrennzeichen_en](https://lp.qvantum-plan.de/hubfs/zahlformatierung_dezimaltrennzeichen_en.png)


Correct input:


![zahlformatierung_dezimaltrennzeichen2](https://lp.qvantum-plan.de/hubfs/zahlformatierung_dezimaltrennzeichen2.png)


### Cell functions


Cell functions can be used. More about [cell functions](https://lp.qvantum-plan.de/en/wissensdatenbank/cell-functions).


### Minus sign


You may use a maximum of one preceding minus. 



A minus sign must not be used with a cell function in the same cell from a form.



Error message with two minus signs:


![zahlformatierung_minus_en](https://lp.qvantum-plan.de/hubfs/zahlformatierung_minus_en.png)


Example:


![zahlformatierung_minus2_en](https://lp.qvantum-plan.de/hubfs/zahlformatierung_minus2_en.png)


### Formatting with units


The string belonging to the value type of the cell to be changed may be used after the number. Each cell has exactly one of 5 possible value types. The owner can define a string as a unit for each of these value types.


Example:


For the value type "Price" the string "EUR" could have been defined and for the value type "Percentage" the string "%". Then the input "3EUR" would be allowed for a "Price" cell. Forbidden for the same cell would be "3€" or "3$" because these are not the specified string in each case, and "3%" is also not allowed because it is not a "percentage" cell. When you leave the cell, we format the number as specified by the owner, from this you can read the correct string.


There may be any number of spaces between the number and the string.


Example:


![zahlformatierung_einheiten_en](https://lp.qvantum-plan.de/hubfs/zahlformatierung_einheiten_en.png)


### Multiplying numbers using K or M


  
The characters **K** and **M** serve as abbreviations for **thousands** and **millions**. 


#### Multiply with thousand (K)



```
<number>K or <number>k multiplies <number> with 1.000
```

Before:


![zellfunktion_k-1200x545](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_k-1200x545.png)


After:


![zellfunktion_k1-1024x486](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_k1-1024x486.png)


#### Multiply with million (M)



```
<number>M or <number>m multiplies <number> with 1.000.000
```

Before:


![zellfunktion_m-1024x486](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_m-1024x486.png)


After:


![zellfunktion_m1](https://lp.qvantum-plan.de/hubfs/Imported%20images/zellfunktion_m1.png)


 


 


 

**Category:** Formulare
**Subcategory:** Arbeiten mit Formularen
**Keywords:** formatting,number formatting
[Original Article](https://lp.qvantum-plan.de/en/wissensdatenbank/number-formatting)
