# Changelog for deployment on demo and production

**Concerning: All demo and production accounts**

### Changelog for deployment to demo and production on**31.01.2024**


* Value types for calculated columns: Calculated columns, in the context of manually configured axes, the controller can now assign a value type to calculated columns/rows and use it to control the display of units and decimal separators.


### Changelog for deployment to demo and production on 23.01.2024


* There is now a question mark icon in the top menu bar in Qvantum, which is linked directly to the knowledge database. The user can use this to jump directly to the appropriate documentation, depending on where they are in Qvantum.
* When creating a new trial tenant, the P&L model is now also available for selection.


### Changelog for deployment to demo and production on 19.12.2023


* The blank line filter in forms is now permanently available
* The bug that sometimes led to the message "Maximum call stack exceeded" for large forms has been fixed
* The API has been expanded to include the option of querying a CSV structure


### Changelog for deployment to demo and production on 07.11.2023


* Forms and the entries in the main menu can now be opened in a new tab.


### Changelog for deployment to demo and production on 09.10.2023


**Excel model template** can now be run **completely in English**


* **Download of the model with English as user language** creates English model throughout ( until then column headers and other parts were still managed in German)
	+ Model has now a **language setting**, which is placed on the first tab below the version number. Until now only **DE** and **EN** have been supported.
* When **uploading the model**, the English column headers are now also interpreted.


### Changelog for deployment to demo and production on 27.09.2023


* Demo:
	+ Setup work for the formula manager: key figures and formulas are now visible on the model tab (formulas are not editable yet).
* Production:
	+ Permission constraint regarding layer nesting has been relaxed.


### Changelog for deployment to demo and production on 06.09.2023


* New feature level nesting
* Various bug fixes


### Changelog for deployment to demo and production on 27.06.2023


* There is now a decimal comma instead of a decimal point
* There are new cell functions, DIV and MUL


### Changelog for deployment to demo and production on 13.06.2023


* Various upgrades of components in use
* Model templates for standard models ("Download Model Template" on the Model tab) have been revised and are now available in a new design
* The new "Changelog" feature can now be activated per tenant (if needed) to track changes to the data.


### Changelog for deployment to demo and production on 02.05.2023


Several bugs fixes in this deployment.


### Changelog for deployment to demo and production on 04.04.2023


* Saving column widths in forms
* English model template download
* Last Improvements to Fix/Pin Navigation (gray box was replaced)
* Last improvements on formatting rows/columns (new icon to delete formatting)
* Minor bugfixes regarding formatting & sheet nesting


### Changelog for deployment to demo and production on 16.03.2023


* Empty folders are no longer displayed for planners


The following features are now active on all environments:


* Formatting of rows and columns in axis types: Dimensional nesting, Sheet nesting, and user-defined. Also for remark columns.
* Sheet nesting has been fundamentally redesigned, it is now (again) possible to expand and collapse parts. This will also be saved.


Formally not included, but already visible:


* If you use QVANTUM in English you get a different model template.


### Changelog for deployment to demo and production on 14.03.2023


* Trial environment: SSSU only in this environment
* Nesting:
	+ Save sheet nesting including unfold state (FT still out!)
	+ Import/export level names including new model templates for SSSU
* Disable mode change for planners (before fixed axis configuration)
* Cut-Off: completely removed
* Bugfixes:
	+ User synchronization
	+ Incorrect/incomplete calculation after model update


### Changelog for deployment to demo and production on 09.02.2023


* **Performance improvements:**
	+ Time required for the model update could be reduced by approx. 50%.
	+ Performance when saving inputs in the frontend could be improved significantly through various optimization methods
* **Merging of aspect and structure** could finally be completed after months. It simplifies future developments and prevents us from building up technical debt.
* **Search function in dimensions**: Multiple hits can now be called one after the other.


### Changelog for deployment to demo and production on 22.12.2022


The following content has gone live:


* Lock, enforce, pin navigation: the controller can restrict the navigation for the planner and reduce the display in the forms to the essentials.
* **Internationalization**: the Qvantum app, as well as our website, including registration via the self-service signup form and an English trial version are now available in English. Some minor corrections are still to follow.
	+ The **contrast** between font and background color highlighted rows or columns have been increased for better readability.
	+ Email addresses were previously **case-sensitive** when logging in. This is also correct according to international guidelines. However, a corresponding error message is now displayed for the user at this point.
* **Consistency** of the application databases has been improved.


### Changelog for deployment to demo and production on 14.12.2022


According to our roadmap, large parts of the "**Fix, Force and Pin Navigation**" project have already been implemented. The functions in detail:  

* In forms, the controller can now fix dimensions that are not in the rows or columns. To do this, he selects a node in the form header and fixes it using the lock symbol. Instead of the dropdown for the selection, the planner now sees the fixed node, which has been provided with a lock.
* The selection of elements in a dimension that is in the rows or columns can now no longer be changed via the form header. However, the setting can still be made via the rows/columns dialog.
* In dimensions, where up to now more than one node sat on the top level, a synthetic node "All" was automatically displayed. Here, the display has now changed to make "All" not look like a node in the structure.
* If a planner has no permissions on the fixed element, the form is invalid for him and is hidden.


### Changelog for deployment to demo and production on 22.11.2022


* Highlights
	+ Further steps for internationalization
	+ Search function for elements in dimensions
	+ Increased modeling power with forest structures


### Changelog for deployment to demo and production on 25.10.2022


* Highlights
	+ Redesign toolbar
	+ Many steps for internationalization
	+ A bug in the backend distribution was fixed


### Changelog for deployment to demo and production on 12.10.2022


* The second nesting (leaves with leaves) is active


### Changelog for deployment to demo and production on 10.10.2022


* Bugfixes


### Changelog for deployment to demo and production on 13.09.2022


* Bugfixes


### Changelog for deployment to demo and production on 05.09.2022


* Bugfixes in editing and deleting forms


### Changelog for deployment to demo and production on 23.08.2022


* Features:
	+ Self-service sign-up including (preliminary) models.
	+ Performance improvements (data upload + query)
	+ Select whole row/column (all first step of "Formatting for Grid Cells")  
	small bugfixes


### Changelog for deployment to demo and production on 09.06.2022


* Features:
	+ Formulas: more functions, operators & constants
		- Functions QUOTIENT & MODULO
		- MIN & MAX functions
		- Boolean functions ISBLANK & ISVALID
		- Boolean operators NOT, AND, OR
		- Constant BLANK


* Bugfixes:
	+ Incorrect calculation in the context of time substitution


### Changelog for deployment to demo and production on 05.04.2022


* DIVIDE and SIGN function
* IF function and thus also comparisons, e.g. IF([A] < [2]; [B]; [C] + 1)
* Forms without authorization on elements (e.g. sales units) are hidden.
* Basic nesting
* Highlight active row/column
* Release forms for all or none or specific planners


### Changelog for deployment to demo and production on 04.05.2022


* Features:
	+ **Conditions in formulas:** The if formula function is available in form and key figure formulas.
	+ **Permissions on forms:** Forms can be authorized for owners/for all planners. A form is automatically hidden for a planner if the planner does not have permissions on all elements of the form row or column definition.


* Bug fixes:
	+ **Highlighting columns/row headers:** the highlighting of columns/row headers related to a focused data cell in the form had an incorrect behavior after scroll operations in larger forms. With this bugfix this was corrected.
	+ **Form saving:** after saving a change to a form, the change was no longer displayed after a form change, only after a page reload. With this bugfix the changes are shown correctly again without page reload.


### Changelog for deployment to demo and production on 05.04.2022



This changelog additionally lists some issues that have been deployed for some time but have not been mentioned in any changelog yet.



* Features:
	+ Form folders: forms can be structured in folders.
	+ Hide empty rows/columns: Form rows/columns that are either completely empty or only filled with 0 values can be shown or hidden using a filter.
	+ Admin SSO: In addition to SSO for planners, SSO is also available for admins of QVANTUM planning applications.
	+ Navigation links on forms: Links on forms can contain additional navigation information to control the set header dimensions.
	+ Input capability enhancement: improved recognition of independent cube ranges now allows significantly more cube cells to be entered in user-defined columns that were previously locked. E.g. the column ACTUAL/Total Year was locked in combination with PLAN/January, even though both columns were located in disjoint subcubes.
	+ Subset filter in data export API: for data requests via the data export API, subset filters can now be formulated over multiple dimension elements per dimension. This allows for more targeted exports of specific cube ranges.


* Bugfixes: Bug in backend aggregation fixed.


### Changelog for deployment to demo and production on 19.01.2022


* INFO: The formula system was prepared in the background for further functions. This may have changed already existing formulas to show the same behavior as before.
* Fixed a bug that prevented the use of the dimension sheet "#Dimension" in the model template.
* Fixed minor graphical bugs on the team tab.


**Category:** Changelogs
**Keywords:** Changelog,Demo,Production,Updates
[Original Article](https://lp.qvantum-plan.de/en/wissensdatenbank/changelog)
