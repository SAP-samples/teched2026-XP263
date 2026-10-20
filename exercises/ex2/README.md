# Exercise 2 - Create the Access Package in Microsoft Entra

In this exercise, you will work as a **Microsoft Entra administrator** and configure the Microsoft Entra ID Governance objects that business users will use to request Procurement Manager access (see *figure 2*).

<br><br>
<a href="./images/ex2.jpg" target="_blank"><img src="./images/ex2.jpg"/></a>

*Figure 1: Exercise 2*<br><br>

Microsoft Entra ID Entitlement Management organizes access through **catalogs**, **resources**, and **access packages**. An access package bundles the resources that a user needs for a particular business purpose and defines the policies governing how that access can be requested and approved.

For this scenario, the SAP Cloud IAG business role `BR_XP263_<NN>` is made available as a resource in the Microsoft Entra catalog. You will include this resource in the `AP_XP263_<NN>` access package together with the Microsoft Entra resources required by the scenario.

You will also configure the access package policy that controls who can request the package and how the request is approved.

At the end of this exercise, the access package is available for eligible business users to request through the Microsoft Entra My Access portal.


| Step   | Description                | Screenshot |
| :----- | :------------------------- | :--------- |
| 01     | Switch back to the **Microsoft Entra admin center** in the first browser tab.<br><br>Navigate to **ID Governance &rarr; Entitlement management**.|<a href="./images/2-1.jpg" target="_blank"><img src="./images/2-1.jpg" width="250"/></a>|
| 02     | Select **Catalogs** from the **Entitlement management** submenu.<br><br>Click **New catalog**.|<a href="./images/2-2.jpg" target="_blank"><img src="./images/2-2.jpg" width="250"/></a>|
| 03     | Enter **`XP263_<NN>`** for the name of the new catalog, and a description, for example "*Catalog for session XP263*". Replace **`<NN>`** with the number of your seat.<br><br>Click **Create**. |<a href="./images/2-3.jpg" target="_blank"><img src="./images/2-3.jpg" width="250"/></a>|
| 04     | Select your new catalog **`XP263_<NN>`** from the list. |<a href="./images/2-4.jpg" target="_blank"><img src="./images/2-4.jpg" width="250"/></a>|
| 05     | Navigate to **Resources** in the menu.<br><br>Click **Add resources**.|<a href="./images/2-5.jpg" target="_blank"><img src="./images/2-5.jpg" width="250"/></a>|
| 06     | Click **Groups and Teams**.|<a href="./images/2-6.jpg" target="_blank"><img src="./images/2-6.jpg" width="250"/></a>|
| 07     | In the search bar, enter "*Procurement*". From the search results, **activate** the checkbox for the group **ProcurementTeam** to select it.<br><br>Click **Select**.|<a href="./images/2-7.jpg" target="_blank"><img src="./images/2-7.jpg" width="250"/></a>|
| 08     | Click **External Resources**.|<a href="./images/2-8.jpg" target="_blank"><img src="./images/2-8.jpg" width="250"/></a>|
| 09     | From the **Connector** drop-down list, select **SAP TechEd XP263**.<br>For **Resource Type**, select **Business Role**.<br><br>Click on the resource **SAP IAG Access Rights** to select it.<br><br>Click **Select**.|<a href="./images/2-9.jpg" target="_blank"><img src="./images/2-9.jpg" width="250"/></a>|
| 10     | Click **Add**. |<a href="./images/2-10.jpg" target="_blank"><img src="./images/2-10.jpg" width="250"/></a>|
| 11     | Navigate to **Access packages** in the menu. Click **New access package**.|<a href="./images/2-11.jpg" target="_blank"><img src="./images/2-11.jpg" width="250"/></a>|
| 12     | Enter **`AP_XP263_<NN>`** for the **Name** of the new acccess package, and provide a **Description** (for example "*Access package for session XP263*).<br><br>Click **Next: Resource roles**.|<a href="./images/2-12.jpg" target="_blank"><img src="./images/2-12.jpg" width="250"/></a>|
| 13     | Click **Groups and Teams**. |<a href="./images/2-13.jpg" target="_blank"><img src="./images/2-13.jpg" width="250"/></a>|
| 14     | **Activate** the checkbox for **ProcurementTeam** from the search results to select it.<br><br>Click **Select**. |<a href="./images/2-14.jpg" target="_blank"><img src="./images/2-14.jpg" width="250"/></a>|
| 15     | From the **Role** drop-down list of the **ProcurementTeam** group resource, select **Member**. |<a href="./images/2-15.jpg" target="_blank"><img src="./images/2-15.jpg" width="250"/></a>|
| 16     | Click **External Resources**. |<a href="./images/2-16.jpg" target="_blank"><img src="./images/2-16.jpg" width="250"/></a>|
| 17     | Click **SAP IAG Access Rights** from the list to select it.<br><br>Click **Select**.|<a href="./images/2-17.jpg" target="_blank"><img src="./images/2-17.jpg" width="250"/></a>|
| 18     | From the **Role** drop-down list of the **SAP IAG Access Rights** business role resource, select the business role **`BR_XP263_<NN>`** you created in the [previous exercise](../ex1/README.md).<br><br>Replace **`<NN>`** with the number of your seat.|<a href="./images/2-18.jpg" target="_blank"><img src="./images/2-18.jpg" width="250"/></a>|
| 19     | Click **Next: Requests**. |<a href="./images/2-19.jpg" target="_blank"><img src="./images/2-19.jpg" width="250"/></a>|
| 20     | For **Who can get access**, select the first option **For users, service principals, and agent identities in your directory**.<br><br>For **Select specific scope**, select the option **Specifc users and groups**.<br><br>Click **+ Add users and groups**. |<a href="./images/2-20.jpg" target="_blank"><img src="./images/2-20.jpg" width="250"/></a>|
| 21     | Enter your business user's name **`user-<NN>`** in the search bar. Replace **`<NN>`** with the number of your seat.<br><br>From the search results, activate the checkbox to select your user.<br><br>Click **Select**.|<a href="./images/2-21.jpg" target="_blank"><img src="./images/2-21.jpg" width="250"/></a>|
| 22     | For **Who can request access**, **activate** the checkbox for **Self**.<br><br>Choose **No** for **Require requestor justification**.<br><br>For the **Approval** settings, select **Yes** to **Require approval**, and **1** for **How many stages**.<br><br>From the **First Approver** drop-down list, select **Choose specific approvers**.<br><br>Click **Add approvers**.|<a href="./images/2-22.jpg" target="_blank"><img src="./images/2-22.jpg" width="250"/></a>|
| 23     | Enter your Entra approver's name **`entra-<NN>`** in the search bar. Replace **`<NN>`** with the number of your seat.<br><br>From the search results, activate the checkbox to select your user.<br><br>Click **Select**. |<a href="./images/2-23.jpg" target="_blank"><img src="./images/2-23.jpg" width="250"/></a>|
| 24     | Choose **No** for **Require approver justification**.<br><br>Choose **Yes** for **Disable assignment emails**.<br><br>Click **Next: Requestor Information**. |<a href="./images/2-24.jpg" target="_blank"><img src="./images/2-24.jpg" width="250"/></a>|
| 25     | Click **Next: Lifecycle**. |<a href="./images/2-25.jpg" target="_blank"><img src="./images/2-25.jpg" width="250"/></a>|
| 26     | Choose **Never** for **Access package assignment expire**.<br><br>Choose **No** for **Users can request specific timeline**.<br><br>Choose **No** for **Allow users to extend access**.<br><br>**Click Review + create**.|<a href="./images/2-26.jpg" target="_blank"><img src="./images/2-26.jpg" width="250"/></a>|
| 27     | Click **Create**. |<a href="./images/2-27.jpg" target="_blank"><img src="./images/2-27.jpg" width="250"/></a>|
| 28     | **Copy** the link of the new **access package** in the **My Access portal** to the clipboard. |<a href="./images/2-28.jpg" target="_blank"><img src="./images/2-28.jpg" width="250"/></a>|


Continue to - [Exercise 3 - Request the access package in Microsoft Entra](../ex3/README.md)
