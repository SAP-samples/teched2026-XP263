# Exercise 2 - Create the Access Package in Microsoft Entra

In this exercise, you will create the following Entra ID Governance objects:
* A **Catalog**, which is a container that groups related *Resources* and *Access Packages*, defining which resources are available to be included in those packages.
* **Resources** are the actual items to which access can be granted, such as an SAP Cloud IAG business role, an Entra group, an applications role, or SharePoint Online sites.
* The **Access Package** provides the user-facing access request and governance layer. It bundles one or more of those catalog resources with policies governing who can request access, approvals, and the access lifecycle.
<br><br>
In this scenario, the **Access Package** includes the SAP Cloud IAG business role with the SAP-specific permissions created in the [previous exercise](../ex1/README.md) alongside the Microsoft resources, which is the role of the Microsoft Azure Web application. Approval for the SAP portion is passed over to SAP Cloud IAG, whereas the process for approving access to the Azure Web application is configured and managed in Entra ID Governance.


| Step   | Description                | Screenshot |
| :----- | :------------------------- | :--------- |
| 01     | Switch back to the **Microsoft Entra admin center** in the first browser tab.<br><br>Navigate to **ID Governance &rarr; Entitlement management**.|<a href="./images/2-1.jpg" target="_blank"><img src="./images/2-1.jpg" width="250"/></a>|
| 02     | Select **Catalogs** from the **Entitlement management** submenu.<br><br>Click **New catalog**.|<a href="./images/2-2.jpg" target="_blank"><img src="./images/2-2.jpg" width="250"/></a>|
| 03     | Enter **`XP263_<NN>`** for the name of the new catalog. |<a href="./images/2-3.jpg" target="_blank"><img src="./images/2-3.jpg" width="250"/></a>|
| 04     | abc |<a href="./images/2-4.jpg" target="_blank"><img src="./images/2-4.jpg" width="250"/></a>|
| 05     | abc |<a href="./images/2-5.jpg" target="_blank"><img src="./images/2-5.jpg" width="250"/></a>|
| 06     | abc |<a href="./images/2-6.jpg" target="_blank"><img src="./images/2-6.jpg" width="250"/></a>|
| 07     | abc |<a href="./images/2-7.jpg" target="_blank"><img src="./images/2-7.jpg" width="250"/></a>|
| 08     | abc |<a href="./images/2-8.jpg" target="_blank"><img src="./images/2-8.jpg" width="250"/></a>|
| 09     | abc |<a href="./images/2-9.jpg" target="_blank"><img src="./images/2-9.jpg" width="250"/></a>|
| 10     | abc |<a href="./images/2-10.jpg" target="_blank"><img src="./images/2-10.jpg" width="250"/></a>|
| 11     | abc |<a href="./images/2-11.jpg" target="_blank"><img src="./images/2-11.jpg" width="250"/></a>|
| 12     | abc |<a href="./images/2-12.jpg" target="_blank"><img src="./images/2-12.jpg" width="250"/></a>|
| 13     | abc |<a href="./images/2-13.jpg" target="_blank"><img src="./images/2-13.jpg" width="250"/></a>|
| 14     | abc |<a href="./images/2-14.jpg" target="_blank"><img src="./images/2-14.jpg" width="250"/></a>|
| 15     | abc |<a href="./images/2-15.jpg" target="_blank"><img src="./images/2-15.jpg" width="250"/></a>|
| 16     | abc |<a href="./images/2-16.jpg" target="_blank"><img src="./images/2-16.jpg" width="250"/></a>|
| 17     | abc |<a href="./images/2-17.jpg" target="_blank"><img src="./images/2-17.jpg" width="250"/></a>|
| 18     | abc |<a href="./images/2-18.jpg" target="_blank"><img src="./images/2-18.jpg" width="250"/></a>|
| 19     | abc |<a href="./images/2-19.jpg" target="_blank"><img src="./images/2-19.jpg" width="250"/></a>|
| 20     | abc |<a href="./images/2-20.jpg" target="_blank"><img src="./images/2-20.jpg" width="250"/></a>|
| 21     | abc |<a href="./images/2-21.jpg" target="_blank"><img src="./images/2-21.jpg" width="250"/></a>|
| 22     | abc |<a href="./images/2-22.jpg" target="_blank"><img src="./images/2-22.jpg" width="250"/></a>|
| 23     | abc |<a href="./images/2-23.jpg" target="_blank"><img src="./images/2-23.jpg" width="250"/></a>|
| 24     | abc |<a href="./images/2-24.jpg" target="_blank"><img src="./images/2-24.jpg" width="250"/></a>|
| 25     | abc |<a href="./images/2-25.jpg" target="_blank"><img src="./images/2-25.jpg" width="250"/></a>|
| 26     | abc |<a href="./images/2-26.jpg" target="_blank"><img src="./images/2-26.jpg" width="250"/></a>|
| 27     | abc |<a href="./images/2-27.jpg" target="_blank"><img src="./images/2-27.jpg" width="250"/></a>|
| 28     | abc |<a href="./images/2-28.jpg" target="_blank"><img src="./images/2-28.jpg" width="250"/></a>|


## Summary

You've now ...

Continue to - [Exercise 3 - Excercise 3 ](../ex3/README.md)
