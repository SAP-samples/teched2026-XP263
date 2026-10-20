# Exercise 6 - Provision and verify user access

In this final exercise, you will complete the end-to-end scenario by provisioning the approved access as the **SAP Cloud IAG administrator** and verifying the resulting user experience as the **business user** (see *figure 1*).

<br><br>
<a href="./images/ex6.jpg" target="_blank"><img src="./images/ex6.jpg"/></a>

*Figure 1: Exercise 6*<br><br>

After the SAP Cloud IAG request has been approved, the access defined by the `BR_XP263_<NN>` business role can be provisioned to the connected target systems. In the scenario, this includes access to **SAP S/4HANA** and the authorization required for the **Purchase Requisition application on SAP BTP**.

You will verify that the required assignments have reached the target systems. In SAP S/4HANA, the user receives the `Z_MM_PURCHASER` role. In the cloud environment, the corresponding authorization enables the **ProcurementManager** role for the Purchase Requisition application.

Finally, you will switch back to the **business user** perspective and verify that the approved access can be used successfully. This closes the access lifecycle that started with the request in Microsoft Entra and continued through approval and provisioning in SAP Cloud IAG.

At the end of this exercise, you will have completed the full scenario.

| Step   | Description                | Screenshot |
| :----- | :------------------------- | :--------- |
| 01     | Go back to the **Google Chrome** browser and switch to the second tab. If your session has already expired, login again to the SAP Cloud IAG tenant with your IAG admin user **`admin-<NN>`**.<br><br>Navigate **back** to the **Home** page of the SAP Cloud IAG Fiori Launchpad.|<a href="./images/6-1.jpg" target="_blank"><img src="./images/6-1.jpg" width="250"/></a>|
| 02     | On the **Home** page, click the **Job Scheduler** tile. |<a href="./images/6-2.jpg" target="_blank"><img src="./images/6-2.jpg" width="250"/></a>|
| 03     | Enter *`XP263_<NN>`* for the **Job Name**.<br><br>Replace **`<NN>`** with the number of your seat.<br><br>Select **Provisioning** from the **Job Category** drop-down list.<br><br>Click **Schedule Job**.|<a href="./images/6-3.jpg" target="_blank"><img src="./images/6-3.jpg" width="250"/></a>|
| 04     | Navigate **back** to the **Home** page. |<a href="./images/6-4.jpg" target="_blank"><img src="./images/6-4.jpg" width="250"/></a>|
| 05     | Click the **Job History List** tile.|<a href="./images/6-5.jpg" target="_blank"><img src="./images/6-5.jpg" width="250"/></a>|
| 06     | Expand the **Provisioning** Job Category and select your job with the name *`XP263_<NN>`* from the list.|<a href="./images/6-6.jpg" target="_blank"><img src="./images/6-6.jpg" width="250"/></a>|
| 07     | Wait for the **Status** to be **Completed**. Click **Refresh** to update the status.<br><br>Then select the job execution from the list and switch to the **Job Logs** tab.<br><br>In the Job Logs, search for two entries reporting successful provisioning of the **ProcurementManager** assignment in the SAP BTP CAP application, and the **Z_MM_PURCHASER** role in the S/4HANA system. |<a href="./images/6-7.jpg" target="_blank"><img src="./images/6-7.jpg" width="250"/></a>|
| 08     | Go back to the **Microsoft Edge browser** and open a new **InPrivate** window. |<a href="./images/6-8.jpg" target="_blank"><img src="./images/6-8.jpg" width="250"/></a>|
| 09     | Go to the [Purchase Requisition App](https://sap-teched-2026-xp263-xp263-6cntx8l6-dev-procurement.cfapps.us20.hana.ondemand.com/) at `https://sap-teched-2026-xp263-xp263-6cntx8l6-dev-procurement.cfapps.us20.hana.ondemand.com/` on SAP BTP.<br><br>Login with your business user's account **`user-<NN>@bestruncorp.onmicrosoft.com`**.<br><br> Replace **`<NN>`** with the number of your seat.<br><br> |<a href="./images/6-9.jpg" target="_blank"><img src="./images/6-9.jpg" width="250"/></a>|
| 10     | Enter the user's password.<br><br>Click **Sign in**.|<a href="./images/6-10.jpg" target="_blank"><img src="./images/6-10.jpg" width="250"/></a>|
| 11     | Click **Next**. |<a href="./images/6-11.jpg" target="_blank"><img src="./images/6-11.jpg" width="250"/></a>|
| 12     | Click **Skip setup**. |<a href="./images/6-12.jpg" target="_blank"><img src="./images/6-12.jpg" width="250"/></a>|
| 13     | Click **Yes**. |<a href="./images/6-13.jpg" target="_blank"><img src="./images/6-13.jpg" width="250"/></a>|
| 14     | You are successfully signed on in the SAP BTP application and are authorized to **manage purchase requisitions**.|<a href="./images/6-14.jpg" target="_blank"><img src="./images/6-14.jpg" width="250"/></a>|
| 15     | Open the Windows **Start** menu on the desktop and launch the **SAP Logon** app.|<a href="./images/6-15.jpg" target="_blank"><img src="./images/6-15.jpg" width="250"/></a>|
| 16     | Select the S/4HANA backend system **HE4** from the list. |<a href="./images/6-16.jpg" target="_blank"><img src="./images/6-16.jpg" width="250"/></a>|
| 17     | Login with your backend system user **`USER-<NN>`**.<br><br> Replace **`<NN>`** with the number of your seat.|<a href="./images/6-17.jpg" target="_blank"><img src="./images/6-17.jpg" width="250"/></a>|
| 18     | Provide a new password of your choice. |<a href="./images/6-18.jpg" target="_blank"><img src="./images/6-18.jpg" width="250"/></a>|
| 19     | You are successfully signed on in the S/4HANA system and authorized to **manage purchase orders**.|<a href="./images/6-19.jpg" target="_blank"><img src="./images/6-19.jpg" width="250"/></a>|
| 20     | In your **Microsoft Edge** browser, go back to the *Microsoft Entra admin center* on the **first** tab.<br><br>Navigate to **Requests** in your access package.<br><br>Verify that the **Status** and **Sub-status** of your business user's access package request are both set to *`Delivered`*.|<a href="./images/6-20.jpg" target="_blank"><img src="./images/6-20.jpg" width="250"/></a>|
| 21     | Navigate to **Entra ID &rarr; Groups**.<br><br>Enter *"Procurement"* in the **search** field.<br><br>Click on the **ProcurementTeam** group in the search results.|<a href="./images/6-21.jpg" target="_blank"><img src="./images/6-21.jpg" width="250"/></a>|
| 22     | Navigate to **Members**.<br><br>Verify that your business user **`user-<NN>`** has been added as a group member.|<a href="./images/6-22.jpg" target="_blank"><img src="./images/6-22.jpg" width="250"/></a>|