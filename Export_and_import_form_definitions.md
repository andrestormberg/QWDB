# Export and import form definitions 

**Export and import forms.**

QVANTUM distinguishes between an export of forms and an export of the form definition. This article is about the export of form definitions.


### Requirements


To export form definitions at least one saved form must exist in your QVANTUM account.


To import form definitions, the model should have changed as little as possible between export and import. Invalid forms, for example, always ensure that the import is not possible without further ado. You must then repair the exported form file.


### Export form definitions


Once the requirements to export form definitions are met, the Export Form Definitions button on the Forms tab becomes active.  
  
Inactive definition export:


Active definition export:


Afterwards click on the download icon. The export will then be prepared and downloaded. It is a file in JSON format that you'll be able to archive.


### Import form definitions


You can perform the form import even if no forms exist so far.


Active definition export:


Click on the Upload icon and then select an export file to upload to the system. A warning message will follow, because the import file will always replace the form that is already present in QVANTUM.


Warning message for import of form definitions:


[![import_message_form_def](https://lp.qvantum-plan.de/hubfs/import_message_form_def.png)](https://lp.qvantum-plan.de/hubfs/import_message_form_def.png)


If the import is successful, you will receive a success message and the new forms will be loaded.  
  
If the import fails, you will receive an error message. The failure can be caused by several reasons:


* The model imported in the account does not match the model used to export.
* There are invalid forms in the export file that cannot be imported.


These cases may be repairable with manual intervention in the exported JSON file.


 


 



**Category:** Formulare
**Subcategory:** Weiteres zu den Konfigurationsmöglichkeiten
**Keywords:** JSON,export,forms,import
[Original Article](https://lp.qvantum-plan.de/en/wissensdatenbank/export-and-import-form-definitions)
