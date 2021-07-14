# AS_Domain_Watchlist

Author: Arbala Security

For any technical questions, please contact info@arbalasystems.com   

This ARM template will create a Watchlist and a Logic App to work in tandem with one another. The Logic App is intended to be run from an Azure Sentinel alert. It will extract the domains from entities in an alert and add them to the watchlist. You will be able to view, edit, or repurpose the watchlist as you see fit.

#
To configure and deploy this playbook:
 
Open your browser and ensure you are logged into your Azure Sentinel workspace. In a separate tab, open the link to our ARM template on the Arbala Security GitHub Repository:

https://github.com/Arbala-Security/AS_Domain_Watchlist

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FArbala-Security%2FAS_Domain_Watchlist%2Fmain%2Fazuredeploy.json" target="_blank">
    <img src="https://aka.ms/deploytoazurebutton""/>
</a>
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FArbala-Security%2FAS_Domain_Watchlist%2Fmaster%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazuregov.png"/>
</a>                                                 

From there, click the “Deploy to Azure” button at the bottom and it will bring you to the Custom Deployment Template.

In the first section:  

* Select the “**Subscription**” and “**Resource Group**” from the dropdown boxes you would like the playbook deployed to.  

In the **Parameters** section:   

* **Playbook Name**: This can be left as “AS_Domain_Watchlist” or you may change it.  

* **WorkspaceName**: Enter the name of the Azure Sentinel Workspace you are using for deplolyment.

* **WatchlistName**: You may keep the default name or change it to something to better suit your usecase.

* **watchlistdescription**:  Enter a description for your watchlist. 

Towards the bottom, click on “Review + create”. 

![Template](Images/template1.png)

Once the resources have validated, click on "Create".

![Template](Images/template2.png)

The resources should take around a minute to deploy. Once the deployment is complete, you can expand the "Deployment details" section to view them.
Click the one corresponding to the Logic App.
