# Formulare mit verschachtelten Ebenen

**Im Modus "Automatisch nach Ebenen" können Ebenen beliebiger Dimensionen ineinander verschachtelt werden.**

Der Modus "Automatisch nach Ebenen" steht jetzt im Dialog zur Konfiguration der Zeilen/Spalten zur Verfügung.


![Abbildung 1 – Der Modus bei der Belegung der Zeilen oder Spalten](https://lp.qvantum-plan.de/hubfs/image-png-Sep-05-2023-01-37-21-7194-PM.png)


*Abbildung 1 – Der Modus bei der Belegung der Zeilen oder Spalten*


Durch das Zusammenführen der hierarchischen Ebenen verschiedener Dimensionen zu einer neuen Struktur bieten sich neue Möglichkeiten für die Formularerstellung. Im nachfolgenden Beispiel wird gezeigt, wie die Verschachtelung von Ebenen funktioniert und wie Sie in nur wenigen Schritten eine neue Struktur für Ihre Zeilen oder Spalten erstellen können.


#### Schritt 1 – Ebenen auswählen


Wählen Sie zuerst im Modus "Automatisch nach Ebenen" eine Dimension aus. In unserem Beispiel orientieren wir uns am Modell der Personalkostenplanung und wählen die Organisationseinheiten. Diese Dimension besteht aus den folgenden Ebenen: Gesamtunternehmen, Bereiche, Kostenstelle/Team und auf der untersten Ebene die Mitarbeiter. Für unser Beispiel entscheiden wir uns für die Ebene 2 (Bereiche).



**Achtung!**


Wenn Sie an dieser Stelle keine Auswahl treffen können, könnte es sein, dass die Ebenen im Modell nicht benannt wurden. In diesem Fall kann durch ein einfaches Modellupdate Abhilfe geschaffen werden. [Hier](https://lp.qvantum-plan.de/wissensdatenbank/modellvorlage#Ebenenname-im-Modell) erfahren Sie, wie es funktioniert.



Anschließend fügen wir die Dimension "Varianten" hinzu. Diese Dimension hat nur eine einzige Ebene, die dann standardmäßig bereits vorausgewählt ist.


Zum Abschluss fügen wir eine weitere Ebene aus der Dimension "Organisationseinheiten" hinzu. Allerdings sind die Kostenstellen in unserem Beispiel weniger relevant, daher fügen wir als dritte Ebene unserer Verschachtelung die Ebene "Mitarbeiter" (Ebene 4 der Organisationseinheiten) hinzu.


![Abbildung 2 – Auswahl einer Ebene (rechts) nach Festlegen einer Dimension (links)](https://lp.qvantum-plan.de/hubfs/image-png-Sep-05-2023-01-38-20-8065-PM.png)


*Abbildung 2 – Auswahl einer Ebene (rechts) nach Festlegen einer Dimension (links)*


 


#### Schritt 2 - Filtern in verschachtelten Ebenen


Im vorliegenden Beispiel betrachten wir die Ausgaben für die Krankenkasse der Mitarbeiter in der Abteilung "Vertrieb". Die Mitarbeiter in anderen Abteilungen sind in diesem Zusammenhang nicht relevant. Nachdem Sie die Ebenen festgelegt haben, öffnen Sie die Kategorie "Filter festlegen", die sich direkt unter den Ebenen im gleichen Dialog befindet. Legen Sie fest, welche Einträge aus welcher Dimension Sie betrachten möchten. In unserem Beispiel wählen wir den "Vertrieb" in der Dimension "Organisationseinheiten".


![Abbildung 3 – Filtern in verschachtelten Ebenen](https://lp.qvantum-plan.de/hubfs/image-png-Sep-05-2023-01-38-43-8483-PM.png)


*Abbildung 3 – Filtern in verschachtelten Ebenen*


#### Schritt 3 – Auswahl für die Belegung der Spalten


Für die Spalten wählen wir jetzt wieder den Modus „Automatisch nach Ebenen“. Als erste Ebene wählen wir Ebene „Quartale“ aus der Dimension „Monate“.


Unser Beispiel sieht vor, die Ausgaben für die Krankenversicherung unserer Vertriebsmitarbeiter gegenüberzustellen. In unserer Kennzahlenstruktur liegt die Kennzahl „Krankenversicherung“ auf Ebene 2 der Kennzahlen (siehe auch Abbildung 4). Da uns andere Kennzahlen in diesem Formular nicht interessieren, legen wir einen Filter auf die Kennzahl „Krankenversicherung“.


*![Abbildung 4 - Die Kategorie Ebenen festlegen (links) und die Kategorie „Filter festlegen“ (rechts) beim Konfigurieren der Spalten ](https://lp.qvantum-plan.de/hubfs/image-png-Sep-05-2023-01-39-02-4582-PM.png)*


*Abbildung 4 - Die Kategorie Ebenen festlegen (links) und die Kategorie „Filter festlegen“ (rechts) beim Konfigurieren der Spalten* 


 


Abbildung 5 zeigt das Resultat unserer Verschachtelung. Die Ausgaben für die Krankenversicherung unserer Vertriebsmitarbeiter werden quartalsweise gelistet. Dabei stellen wir IST- und Plan-Variante gegenüber.


![Abbildung 5 – Ausgaben für die Krankenversicherung der Vertriebsmitarbeiter werden auf Quartalsebene gelistet. IST- und Plan-Variante werden verglichen. ](https://lp.qvantum-plan.de/hubfs/image-png-Sep-05-2023-01-39-09-9842-PM.png)


*Abbildung 5 – Ausgaben für die Krankenversicherung der Vertriebsmitarbeiter werden auf Quartalsebene gelistet. IST- und Plan-Variante werden verglichen*. 



**Category:** Formulare
**Subcategory:** Weiteres zu den Konfigurationsmöglichkeiten
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/wie-baue-ich-ein-formular-mit-verschachtelten-ebenen)
