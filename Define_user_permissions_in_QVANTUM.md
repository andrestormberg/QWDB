# Define user permissions in QVANTUM

**Define permissions via CSV upload
**

By uploading the permissions as a CSV you can adjust the permissions of your entiere team at once. Only requirement is that you have already imported master data of your team.


In the permissions CSV, there are three "base columns" that have to be set at all times.





| **email** | **dimension name** | **input** |



The columns "[dimension name]" and "input" are relevant for the permissions.



Note: All users that are not explicitly listed in the authorization CSV lose all previously existing authorizations in QVANTUM after the import.



### Column "[Dimension name]"


This column is a placeholder that must be filled with the name of the dimension with the role "Planning units". By using the permissions export, the name of the dimension will be set automatically.


#### Special features of the dimension with the role "Planning units"


There must be one dimension per model that has the role "Planning unit". This defines the basic permissions for the users, which is also used for the workflow. Each user must be assigned to one element of this dimension.


Even the root node (e.g. "All Sales Units") can be defined as an permission by either permitting the exact element or writing the keyword "all" (without quotes or square brackets) in the affected column.  
  
Example CSV for permissions:


![csv_ausgefüllt_en](https://lp.qvantum-plan.de/hubfs/csv_ausgef%C3%BCllt_en.png)


### Column  for "Input"


The value yes (alternatives: yes or y) indicate that the "read and write" permission is set. Value no (alternatives: no or n) indicate that only the permission to read values is present.


The actual permissions are defined as a separate column in the CSV. For this purpose, the singular name of the dimension is used as the column header, e.g. "Sales Unit" or "Product". The keys of the dimension elements are then entered as values of the column.


### Authorize on multiple elements of a dimension


You can also set permissions on more than one element of a dimension. This can be done in two ways:


1. Authorize a user on an element with hierarchically subordinate elements ("nodes"): The user is automatically authorized on all subordinate nodes. Just specify the key of the top-level element you want to authorize on.
2. Manually authorize a user on multiple elements: To do this, enter any number of keys of the dimension in a column. Individual keys are separated by square brackets. They can be single or hierarchical elements. The example "[Product1] [Product2] [Productgroup 2]" in the column "Product" authorizes on the single products 1 and 2 and additionally on the product group 2.


In all dimensions except the dimension with the role "Planning units" applies: If a value for a user is left empty, the authorization automatically applies to all elements of the dimension.


 


 



**Category:** Team
**Subcategory:** Nutzer-Berechtigungen
**Keywords:** User,permissions
[Original Article](https://lp.qvantum-plan.de/en/wissensdatenbank/define-user-permissions-in-qvantum)
