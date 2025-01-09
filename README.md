# MicrosoftGraphForSharePoint
How to use Microsoft Graph API to access SharePoint Sites and Drives from Postman

To run the postman requests -
1) Install Postman v11.23.3 or latest (older version may work as well)
2) Import environment from file Dev.postman_environment.json
3) Import collection from file MicrosoftGraphAPI.postman_collection.json
4) Register an app in Microsoft Entra Id with Delegated permission type for User.Read and Sites.ReadWrite.All. Be sure to grant admin consent for Sites.ReadWrite.All.
5) Update the env variables for TenantID, ClientID, ClientSecret, UserID, UserPassword. Rest of the variables are populated by script embedded in request.
6) Make sure the UserID used to get GetTokenROPC has read and/or readwrite access to the SharePoint site you are testing (if you are using delegated permissions for graph api)
