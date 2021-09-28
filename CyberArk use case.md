# CyberArk Use Case


```{admonition} How Architecture going to look

1. Assuming each customer network has access to Central Credential Provider to get the Password for a given Resource and Login-account
2. We going to create an APP for CyberArk Integration in which customer can give the API url to test the connection between OpsRamp and to there CyberArk Central Credential Provider.
3. Once the Connection is successful, that means the Integration works and Customer need to provide basic information in the API URL to fetch the Credentials from the Vault.
4. In OpsRamp UI, we going to have an option to pass the API and get the credentials at Remote console or in the Discovery and Monitoring or any where in the platform where Authentication is required

```
Web Based Rest API URL

>CyberArk uses web based api to fetch the authntication details

CyberArk Rest API’s
>[Rest API details](https://services-uscentral.skytap.com:{{port}}/AIMWebService/api/Accounts?appid={parm}&safe={parm}&Query=Database={parm};UserName={parm};Address={parm}
)


The Minimum to get a result back should be:
>The appID, the Safe, declare Query and at least one parameter from the list [in this link](https://docs.cyberark.com/Product-Doc/OnlineHelp/AAM-CP/Latest/en/Content/CCP/Calling-the-Web-Service-using-REST.htm)
