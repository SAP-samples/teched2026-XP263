# Exercise 1 - Create business role in SAP Cloud IAG

In this exercise, you will work as an **SAP Cloud IAG administrator** and create the business role that represents the access required by a Procurement Specialist (see *figure 1*).

<br><br>
<a href="./images/ex1.jpg" target="_blank"><img src="./images/ex1.jpg"/></a>

*Figure 1: Exercise 1*<br><br>

Business roles in SAP Cloud IAG provide a business-oriented abstraction of technical access. Instead of requesting individual application authorizations, access can be grouped into a role representing the responsibilities of a particular business function.

For this scenario, you will configure the business role `BR_XP263_<NN>`, with `<NN>` being replaced by the number of your seat. The role represents the SAP-specific access for the Procurement Specialist function and will later be requested through Microsoft Entra.

This business role is the central link between the Microsoft Entra access governance process and the SAP-specific access governance and provisioning process.

At the end of this exercise, the SAP Cloud IAG business role is ready to be exposed to Microsoft Entra and included in an access package.


| Step   | Description                | Screenshot |
| :----- | :------------------------- | :--------- |
| 01     | Open a **new tab** in the Chrome browser. |<a href="./images/1-1.jpg" target="_blank"><img src="./images/1-1.jpg" width="250"/></a>|
| 02     | Go to the SAP Cloud IAG tenant URL [https://xp263-6cntx8l6.sapciag-ee.cfapps.us20.hana.ondemand.com](https://xp263-6cntx8l6.sapciag-ee.cfapps.us20.hana.ondemand.com).<br><br>To login, **click** the first identity provider (**axzamhxt8.accounts.ondemand.com**) from the list. |<a href="./images/1-2.jpg" target="_blank"><img src="./images/1-2.jpg" width="250"/></a>|
| 03     | Your are single-signed on to the SAP Cloud IAG tenant's Fiori launchpad with your **`admin-<NN>`** user.<br><br>Switch to the **Role Designer** tab. Launch the **Business Roles** app.|<a href="./images/1-3.jpg" target="_blank"><img src="./images/1-3.jpg" width="250"/></a>|
| 04     | Click **Create**. |<a href="./images/1-4.jpg" target="_blank"><img src="./images/1-4.jpg" width="250"/></a>|
| 05     | For the business role name, enter **`BR_XP263_<NN>`**. Replace **`<NN>`** with the number of your seat.<br><br>Provide a **Description**, for example "*Business role for SAP access governance*".<br><br>In the **Business process** drop-down list, select **GLOBAL Business Process**.<br><br>On the **Access** tab, click **Add**.|<a href="./images/1-5.jpg" target="_blank"><img src="./images/1-5.jpg" width="250"/></a>|
| 06     | Enter **`Z_MM`** in the **Search Access** search bar and click the **magnifying glass** symbol.<br><br>From the search results, click **Add** on the **Z_MM_PURCHASER** entry for the *S4HANA_HE4* application.|<a href="./images/1-6.jpg" target="_blank"><img src="./images/1-6.jpg" width="250"/></a>|
| 07     | Repeat the previous step by entering **`ProcurementManager`** in the search bar and click the **magnifying glass** symbol.<br><br>From the search results, click **Add** on the **cap - ProcurementManager** entry for the *SCI_TENANT_AXZAMHXT8* application.|<a href="./images/1-7.jpg" target="_blank"><img src="./images/1-7.jpg" width="250"/></a>|
| 08     | You've now added the technical permissions from the S/4HANA on-premises system and the SAP BTP CAP application to your new business role.<br><br>Click **Close**. |<a href="./images/1-8.jpg" target="_blank"><img src="./images/1-8.jpg" width="250"/></a>|
| 09     | Switch to the **Other attributes** tab.<br><br>Click on the **value help** of the **Content Approvers** field.|<a href="./images/1-9.jpg" target="_blank"><img src="./images/1-9.jpg" width="250"/></a>|
| 10     | Select the **Approver Content (P000088)** user from the list.<br><br>Click **Select**. |<a href="./images/1-10.jpg" target="_blank"><img src="./images/1-10.jpg" width="250"/></a>|
| 11     | Click on the **value help** of the **Assignment Approvers** field.|<a href="./images/1-11.jpg" target="_blank"><img src="./images/1-11.jpg" width="250"/></a>|
| 12     | Enter **`Approver<NN>`** in the search bar and click the **magnifying glass** symbol. Replace **`<NN>`** with the number of your seat.<br><br>Select the user **`Approver<NN> IAG`** from the list and click **Select**.|<a href="./images/1-12.jpg" target="_blank"><img src="./images/1-12.jpg" width="250"/></a>|
| 13     | From the **Business subprocess** drop-down list, select **`GLOBAL Sub Process`**.<br><br>From the **Criticality** drop-down list, select **Low**.<br><br>Click **Save and Activate**.|<a href="./images/1-13.jpg" target="_blank"><img src="./images/1-13.jpg" width="250"/></a>|

Continue to - [Exercise 2 - Create the Access Package in Microsoft Entra](../ex2/README.md)