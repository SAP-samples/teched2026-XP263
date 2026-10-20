# Exercise 5 - Approve the access request in SAP Cloud IAG

In this exercise, you will act as the **SAP Cloud IAG approver** and perform the second governance step in the end-to-end access request process (see *figure 1*).

<br><br>
<a href="./images/ex5.jpg" target="_blank"><img src="./images/ex5.jpg"/></a>

*Figure 1: Exercise 5*<br><br>

While Microsoft Entra governs the user's entitlement to the access package, SAP Cloud IAG applies SAP-specific governance to the requested business role. This allows the SAP access to remain subject to the governance processes defined for the SAP environment.

The approved Microsoft Entra request results in an access request for the `BR_XP263_<NN>` business role in SAP Cloud IAG. You will open the request, review the requested access, and approve it using the SAP Cloud IAG approval workflow.

This represents the second approval level in the scenario: first the entitlement is approved in Microsoft Entra, then the SAP business role is approved in SAP Cloud IAG.

At the end of this exercise, all required approvals are complete and SAP Cloud IAG can provision the access contained in the business role to the respective target systems.

| Step   | Description                | Screenshot |
| :----- | :------------------------- | :--------- |
| 01     | Open a **new tab** in the Microsoft Edge browser. |<a href="./images/5-1.jpg" target="_blank"><img src="./images/5-1.jpg" width="250"/></a>|
| 02     | Go to the SAP Cloud IAG tenant URL [https://xp263-6cntx8l6.sapciag-ee.cfapps.us20.hana.ondemand.com](https://xp263-6cntx8l6.sapciag-ee.cfapps.us20.hana.ondemand.com).<br><br>To login, **click** the first identity provider (**axzamhxt8.accounts.ondemand.com**) from the list. |<a href="./images/5-2.jpg" target="_blank"><img src="./images/5-2.jpg" width="250"/></a>|
| 03     | Click **Use another account**. |<a href="./images/5-3.jpg" target="_blank"><img src="./images/5-3.jpg" width="250"/></a>|
| 04     | Enter your IAG approver's username **`iag-<NN>@bestruncorp.onmicrosoft.com`**.<br><br>Replace **`<NN>`** with the number of your seat.<br><br>Click **Next**.|<a href="./images/5-4.jpg" target="_blank"><img src="./images/5-4.jpg" width="250"/></a>|
| 05     | Enter the password.<br><br>Click **Sign in**. |<a href="./images/5-5.jpg" target="_blank"><img src="./images/5-5.jpg" width="250"/></a>|
| 06     | Click **Next**. |<a href="./images/5-6.jpg" target="_blank"><img src="./images/5-6.jpg" width="250"/></a>|
| 07     | Click on your **IAG approver's** account **`iag-<NN>@bestruncorp.onmicrosoft.com`**. |<a href="./images/5-7.jpg" target="_blank"><img src="./images/5-7.jpg" width="250"/></a>|
| 08     | Click **Skip setup**. |<a href="./images/5-8.jpg" target="_blank"><img src="./images/5-8.jpg" width="250"/></a>|
| 09     | Click **Yes**. |<a href="./images/5-9.jpg" target="_blank"><img src="./images/5-9.jpg" width="250"/></a>|
| 10     | Click the **Access Request Inbox** tile. |<a href="./images/5-10.jpg" target="_blank"><img src="./images/5-10.jpg" width="250"/></a>|
| 11     | Select your business user's access request from the list. |<a href="./images/5-11.jpg" target="_blank"><img src="./images/5-11.jpg" width="250"/></a>|
| 12     | Select **Approve** and click **Submit**. |<a href="./images/5-12.jpg" target="_blank"><img src="./images/5-12.jpg" width="250"/></a>|

Continue to - [Exercise 6 - Provision and verify user access](../ex6/README.md)
