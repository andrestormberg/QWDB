# Guide: Assign user permissions

**With the QVANTUM update of 04.10.2021 we change the way user permissions have to be defined in the CSV and via the interface. This guide shows you how to proceed from now on.**

Requirement is that you have already worked with Team-CSV once and you know how to set permissions on dimension elements (more about that here).


### You'll have to take action in the following cases


* If you want to authorize an element (and any elements below it), this element must be written in square brackets (e.g. [North] or [P10299]). The previous notation without square brackets is no longer valid.
* If you use the permissions in multiple dimensions, you can now additionally use the password "ALL" (or "all", "ALL", "all") to automatically authorize all available elements of the dimension. (Previously this had been possible by using an "empty column" in the permissions).
* Empty columns now mean that for this user there should be no more permissions available on this dimension. Attention: This leads to the fact that the user will generally no longer have access to the planning in QVANTUM.



Older CSV files also become invalid as the generic column heading "planning-unit" is no longer supported. Instead, the name of the planning unit dimension must be used. This is automatically taken into account in the team export.


More info: Creating users in QVANTUM.



### Why did these adjustments become necessary?


We are currently simplifying our user management internally to give you better ways to manage and grow your team in the future. With this update, we have laid a foundation for features such as interactive user management without CSV files, easier SSO connection and multiple scheduling without changing accounts.



**Category:** Team
**Keywords:** CSV,User,permissions,planning units
[Original Article](https://lp.qvantum-plan.de/en/wissensdatenbank/guide-assign-user-permissions)
