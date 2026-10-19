# Exercise 2 - Create the Access Package in Microsoft Entra

In this exercise, you will work as a **Microsoft Entra administrator** and configure the Microsoft Entra ID Governance objects that business users will use to request Procurement Manager access (see *figure 2*).

<br><br>
<a href="./images/ex2.jpg" target="_blank"><img src="./images/ex2.jpg" width="250"/></a>

*Figure 1: Exercise 2*<br><br>

Microsoft Entra entitlement management organizes access through **catalogs**, **resources**, and **access packages**. An access package bundles the resources that a user needs for a particular business purpose and defines the policies governing how that access can be requested and approved.

For this scenario, the SAP Cloud IAG business role `BR_XP263_<NN>` is made available as a resource in the Microsoft Entra catalog. You will include this resource in the `AP_XP263_<NN>` access package together with the Microsoft Entra resources required by the scenario.

You will also configure the access package policy that controls who can request the package and how the request is approved.

At the end of this exercise, the access package is available for eligible business users to request through the Microsoft Entra My Access portal.


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


Continue to - [Exercise 3 - Request the access package in Microsoft Entra](../ex3/README.md)
