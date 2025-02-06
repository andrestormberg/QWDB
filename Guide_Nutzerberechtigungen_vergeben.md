# Guide: Nutzerberechtigungen vergeben

**Mit dem QVANTUM-Update vom 04.10.2021 verändern wir die Art und Weise, wie Nutzerberechtigungen im CSV und über die Schnittstelle definiert werden müssen. Dieser Guide zeigt Ihnen, wie Sie ab sofort vorgehen müssen.**

Voraussetzung ist, dass Sie bereits einmal mit dem Team-CSV gearbeitet haben und Sie wissen, wie Berechtigungen auf Dimensionselemente gelegt werden können ([dazu hier mehr](https://lp.qvantum-plan.de/wissensdatenbank/tab-team)).


### Sie müssen in folgenden Fällen aktiv werden


* Wenn Sie ein Element (und ggf. darunter liegende Elemente) berechtigen möchten, muss dieses Element ab sofort in eckigen Klammern (z. B. [Nord] oder [P10299] geschrieben werden. **Die bisherige Schreibweise ohne eckige Klammern ist nicht mehr gültig.**
* Wenn Sie die [Berechtigungen in mehreren Dimensionen nutzen](https://lp.qvantum-plan.de/wissensdatenbank/nutzer-berechtigungen-in-qvantum-definieren), können Sie ab sofort zusätzlich das Kennwort „ALLE“ (oder „alle“, „ALL“, „all“) benutzen, um automatisch alle verfügbaren Elemente der Dimension zu berechtigen. (Bisher war dies durch eine „leere Spalte“ in der Berechtigung möglich gewesen).
* Leere Spalten bedeuten nun, dass für diesen Nutzer **explizit keine** Berechtigungen mehr auf dieser Dimension vorhanden sein sollen. Achtung: Dies führt dazu, dass der Nutzer generell keinen Zugriff mehr auf Ihre QVANTUM-Planung haben wird.



**Hinweis:** Ältere CSV-Dateien sind ebenfalls ungültig geworden, da die generische Spaltenüberschrift „planning-unit“ nun nicht mehr unterstützt wird. Stattdessen muss der Name der Planungseinheiten-Dimension verwendet werden. Dies wird im Team-Export automatisch berücksichtigt.


Mehr Infos: [Benutzer anlegen in QVANTUM](https://lp.qvantum-plan.de/wissensdatenbank/tab-team).



### Warum wurden diese Anpassungen notwendig?


Wir vereinfachen derzeit intern unsere Nutzerverwaltung, um Ihnen in Zukunft bessere Möglichkeiten zu bieten, Ihr Team zu verwalten und zu erweitern. Mit diesem Update haben wir einen Grundstein für Features wie eine interaktive Nutzerverwaltung ohne CSV-Dateien, einfachere SSO-Anbindung und mehrere Planungen ohne Accountwechsel geschaffen.  
  




**Category:** Team
**Keywords:** Benutzer,Berechtigungen,CSV,Nutzer,Planungseinheiten,berechti
[Original Article](https://lp.qvantum-plan.de/wissensdatenbank/guide-nutzerberechtigungen-vergeben)
