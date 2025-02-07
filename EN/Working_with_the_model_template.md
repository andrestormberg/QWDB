# Working with the model template

**Define and upload the planning model, define dimension properties and dimensions.**

The model template supports you in defining your model based on an example for sales planning. The following instructions describe the procedure step by step.  
  
Essentially, defining your planning consists of two steps. First, you fill in the tabs of this Excel sheet according to your desired planning using your own inputs as well as imports from your preliminary systems, thus defining your planning model. Then you upload this Excel file to bring your planning model to life in the QVANTUM Cloud.  
  
Where you can find this file is described on the "[Model](https://lp.qvantum-plan.de/en/wissensdatenbank/tab-model)" page.


### Definition of the planning model


Use the Excel sheet to guide you through the definition of your planning model. Step by step, fill each sheet with your planning metadata. Here is another guide per sheet with important tips on how to proceed:


**- Assistance**


Please pay attention to the provided comments, which will help you to understand and use this template correctly.


**- The sheet Planning Model**  
Start with the Planning Model sheet. On this sheet you define your model in multidimensional form. The dimensions should cover all aspects of your planning. Check that this template contains all the dimensions you need. New dimensions can be added and unneeded dimensions can be removed. Please note that at least the dimension roles "Planning Units" and "Key Figures" must be present for the upload to work.


**- One sheet for each dimension**  
For each dimension, this template contains a separate sheet (e.g. sales units) on which the required dimension elements and, if applicable, their hierarchical relationships are defined. In addition to direct entry, it is possible to obtain this information from other sources using Excel's data integration functions and transfer it to the sheet using "Insert values". Using the Excel function "Insert values" ensures that the plausibility checks stored in the dimension sheet are not overwritten. If you want to create a new dimension, you should first enter it in the Planning Model sheet and then create a new sheet for this dimension. For the creation of the new sheet it is necessary that you copy the sheet #Dimension or #Dimension\_key figure and then rename it according to the plural designation deposited in the sheet planning model.


### Upload the planning application


Once you have completed this template according to your requirements and saved it (under a custom name) as an Excel model file, you can switch back to the QVANTUM web application and upload this model definition. Afterwards, the uploaded model will be available to you for further editing in the cloud.  
  
Next steps:  
If the model generated in QVANTUM does not yet meet your (final) requirements, you can make any necessary changes directly in your Excel file and repeat the upload. If you want to import data (e.g. actual data of past periods) into the model, you can download a data import template that fits your model, fill it with data and upload it again. If the model meets your expectations, you open your QVANTUM web application and continue preparing your planning there. Upload your users in the tab "Team", they will automatically receive a mail with an invitation link when starting the planning. Once the users have entered their planning data, you can finish planning in QVANTUM and retrieve your export reports.


### What is the "planning model"?


A planning model describes an application in the form of a multidimensional cube. The dimensions of the cube should cover all aspects of your planning. This ensures that you can view and manipulate your data from all required perspectives and in various levels of detail.  
  
Each data element (i.e. each number) in this multidimensional cube is uniquely assigned to one element per dimension. These dimension elements thus vividly correspond to the coordinates of a cube cell in which the data element is stored.  
  
Check if this template contains all dimensions you need. New dimensions can be added and unneeded dimensions can be removed.


![vorlage_planungsmodell](https://lp.qvantum-plan.de/hubfs/Imported%20images/vorlage_planungsmodell.png)


Modeling with QVANTUM provides a cube with the following list of dimensions, which you can adjust and extend as needed. For each dimension a sheet (tab see below) is provided in this template. The following list explains what input we'll need from you.   
  
First of all, you need to define a **model abbreviation** and a **model name**. The model abbreviation is used to uniquely identify your design. If, for example, you want to change the designation of your planning later, this is done by specifying this abbreviation. The model designation is the name of your planning model. It is displayed in QVANTUM at different places. **Model description**: here you can enter an additional description for your planning model. This field is not mandatory.  
  
Your planning model consists of different dimensions, which you can define in the table on the Planning Model sheet. You can define different properties for each dimension.


### Dimension properties


The **number** is used to uniquely identify the dimension in the planning model. If, for example, you subsequently want to change the name of your dimension, this is done by specifying this number. Your planning model consists of different dimensions.  
  
**Dimension name**: These dimensions appear in QVANTUM in different places with singular or plural names. Here you can specify the designations. For each dimension you have to define another sheet in the Excel file. This sheet has the plural name of the dimension and there you can define dimension elements.  
  
**Dimension roles**: There are dimensions that take over special tasks in your planning. These dimensions are identified by the dimension roles.  
  
The following dimension roles exist:  
  
**Key figures (mandatory)**: The dimension that identifies your key figures. Key figures are the quantitative contents that are typically mapped in controlling, such as sales quantities, revenues, costs. These key figures can be assigned to so-called value types (amount, quantity, price, percentage), which must be specified on the Excel sheet for this dimension. This dimension can also contain formulas for calculating derived elements, e.g. sales revenue.  
  
**Planning units (mandatory)**: The dimension with the dimension role Planning Units covers the organizational aspect for planning. It is closely related to user authorization. Planning users are assigned the planning units for which they are to enter planning figures.  
  
**Without special role**: You can assign this role to all other dimensions.


### Define dimensions


If you want to create a new dimension, you should first enter it in the Planning Model sheet and then create a new sheet for this dimension. For the creation of the new sheet it is necessary that you copy this sheet **#Dimension** and then rename it according to the plural designation deposited in the sheet planning model.


![vorlage_vertriebseinheiten](https://lp.qvantum-plan.de/hubfs/Imported%20images/vorlage_vertriebseinheiten.png)


### Key


In this column you enter the key of your dimension elements. Keys must be unique per dimension, i.e. there must not be multiple rows that have the same value in the Key column. All characters are allowed. 


### Parent key


To get hierarchical dimensions, you can define a parent element for each element in this column. This element must already have been entered as a key above in the table before it is used. Different elements may have the same parent element, but only one element may be on the top level. This must be in the first row and the field for "parent key" must be empty.  
  
You also have the option to select parent elements from a list. To do this, click on the arrow next to the cell in a row. Now all elements that are already defined above will be displayed.  
  
If you want to have a flat dimension instead of a hierarchical dimension, leave the column "parent key" empty in each row. This way, all elements will be created at the top level.


### Label


In this column you can define the name of your elements. 


### Input allowed?


Here you can specify for each dimension element whether data may be entered for it in the planning model.  
  
**Note**: Please note that data input in the multidimensional cube of the planning model is only possible if all dimension elements assigned to a cube cell have the setting "**Yes**" for "Input allowed?". Select the setting "**No**" if you want to ensure that no input should be made on the dimension element regardless of the combination with elements of other dimensions.  
  
In addition, the input possibility can be limited by other settings such as the authorization of the user or the definition of the form used for the input.  
  
However, data that cannot be entered in principle can either be uploaded or calculated from other data.


### Description


In this column, it is possible to additionally store a description per dimension element. This field is not mandatory.


### Aggregation


If you select the value "Sum" for a dimension element in this column or leave the field empty, this element will be calculated by summing the dimension elements that refer to this element in the column "Parent value". If you do not want summation to take place, you can enter the value "Do not aggregate". 


### Formula


This property may only be assigned in the dimension with the role **Key figures**. If you use the aggregation "Free formula", you can store the formula in this field.   
  
Allowed arithmetic operations (symbol):  
Addition (+)  
Subtraction (-)  
Multiplication (*)  
Division ( / )  
Round brackets  
  
If you want to access other elements in this dimension in a formula, you put the value of the "Key" column in square brackets,  
  
For example: Key figure revenue = [US]*[PPU].  
US = Key of  "Units sold"  
PPU = Key of  "Price per Unit"



**Category:** Modell
**Subcategory:** Arbeiten mit der Modellvorlage
**Keywords:** Aggregation,Dimension,formula,model,model template
[Original Article](https://lp.qvantum-plan.de/en/wissensdatenbank/model-template)
