# Der Workflow

**Vom Starten der Planung über Statusupdates bis zum Abschluss. **

### 


### Abhängigkeiten vom Planungsstatus


Es ist wichtig zu verstehen, dass viele Funktionen in Qvantum erst möglich sind, wenn die Planung gestartet wurde. Anpassungen am Modell oder Veränderungen an einer Struktur können nicht in der aktiven Planungsphase durchgeführt werden, da in der Folge oft der ganze Würfel neu gerechnet werden muss.   


Die folgende Tabelle zeigt, welche Auswirkungen das Starten, Pausieren oder Beenden der Planung haben.




| **Status** | **Auswirkungen auf Controller/Owner** | **Auswirkungen auf Planer** |
| Planung in Vorbereitung     | Ein Controller kann die einzelnen Planungselemente (Modell, Daten, Team und Formulare) vorbereiten.     | Planer haben in diesem Status keinen Zugriff auf QVANTUM. |
| Planung gestartet | Die Planung ist für das eingeladene Team freigegeben. Es können keine Änderungen an den Planungselementen Modell, Daten und Team vorgenommen werden. Formulare können trotzdem weiterhin angepasst werden.     | Planer erhalten ihre Zugangsdaten und können mit der Werteeingabe beginnen. |
| Planung pausiert | Ein Controller kann die einzelnen Planungselemente (Modell, Daten, Team) anpassen.  | Die Eingabe von Werten ist für Planer temporär nicht möglich. |
| Planung beendet | Die Planung kann durch Planer nicht mehr modifiziert werden. Soll eine neue Planung vorbereitet werden, wird vorher nach einem Export der eingegebenen Werte gefragt.     | Die Eingabe von Werten ist für Planer bis zur nächsten Planung nicht möglich. |
| Planung beendet, exportiert | Die Planung kann durch Planer nicht mehr modifiziert werden und der aktuelle Stand der Daten wurde exportiert.     | Die Eingabe von Werten ist für Planer bis zur nächsten Planung nicht möglich. |


### 


### Start des Workflows


Mit Starten einer Planung werden die Zugänge der Planer aktiviert. Planer können sich jetzt einloggen und ihre Planwerte eintragen. Außerdem wird dem Planer jetzt der Planungsstatus (siehe Abbildung 1) angezeigt.



Erst wenn die Planung aktiviert wurde, sehen die Planer das für den Workflow wichtige Feld "Planungsstatus" in der oberen Menüleiste.



### Der Planungsstatus der Planer


Der Ablauf für den Planer gestaltet sich äußerst einfach. In der oberen Menüleiste wird nun der Planungsstatus angezeigt, der zu Beginn auf "Offen" steht. Sobald ein Planer alle erforderlichen Zahlen eingetragen hat, kann er seinen Status auf "Abgeschlossen" setzen. Es ist wichtig zu beachten, dass dieser Statuswechsel nur seinen Teil der Planung betrifft. Für die anderen Planer bleibt der Status unverändert "offen".


 


![image-png-Feb-07-2024-11-51-30-8192-AM](https://lp.qvantum-plan.de/hubfs/image-png-Feb-07-2024-11-51-30-8192-AM.png)


*Abbildung 1 - Das Feld "Planungsstatus" (sichtbar nur für Planer)*


Der Planer kann den Status nur von **"Offen"** auf **"Abgeschlossen"** setzen. Wird der Status **"Pausiert"** angezeigt, bedeutet das, dass der Owner die gesamte Planung pausiert hat. In dieser Zeit können keine weiteren Zahlen eingetragen werden.



Setzt der Planer seinen Status auf "Abgeschlossen" kann er **keine weiteren Änderungen** mehr vornehmen. Sollte das trotzdem erforderlich sein, muss er sich an den Owner wenden, der seinen Zugang wieder freigeben und den Status für ihn damit wieder auf "Offen" setzen kann.



### Die Übersicht über die gesamte Planung für den Owner


Als Owner können Sie selbst keinen Status setzen und auch das Feld "Status" in der oberen Menüleiste entfällt. Dafür sehen Sie auf dem **Teams-Tab** jetzt, welche der Planer ihre Arbeit bereits eingereicht haben und bei wem der Status noch auf "Offen" steht.


Nachdem Sie die Arbeit der Planer überprüft haben, können Sie den Status auf **"Abgenommen"** setzen. Dadurch behalten Sie den Überblick darüber, welche Planungen Sie bereits geprüft haben und welche noch ausstehen. Der Planer hat keine Berechtigung, den Status auf "Abgenommen" zu ändern. Diese Funktion ist ausschließlich für den Owner gedacht, um eine bessere Übersicht auf der Team-Seite zu gewährleisten.


Außerdem haben Sie die Möglichkeit, einem Planer, der seine Planung bereits abgeschlossen hatte, erneut Zugang zu geben. Das kann z.B. erforderlich sein, wenn einer der Planer auf sie zukommt und darum bittet, Korrekturen vornehmen zu dürfen.  


 



**Category:** Übersicht über die Planung
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/der-workflow-in-qvantum)
