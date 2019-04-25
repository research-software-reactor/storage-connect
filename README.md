# storage-connect
Secure cloud data storage for mobile/web apps with ASP.NET API    

## Adapting Storage Connect to the Azure Cloud for use by Mobile Applications

Here within The University of Manchester's RSE team, Andrew Jerrison has developed a web service that supports our development of mobile apps (and web apps) for researchers that typically need a backend SQL database, but only need to store and retrieve data. It is called Storage Connect and its documentation has recently been extracted from the first mobile app that it was used with by Adrian Harwood <https://www.dropbox.com/s/aazrmooihydsv05/Storage_Connect_Specification_20190416.docx?dl=0>. 

Storage Connect's API abstracts away the SQL needed so that mobile app developers can simply use RESTful HTTP calls. Further, data in Storage Connect can also be exported to a Dropbox account.

Currently, Storage Connect runs on a on-premise UoM server and similarly connects to a on-premise SQL Server database.

### Objective 1: Implement Storage Connect on the Azure Cloud.
This will provide several design choices as Azure doubtless provides some (most?) of the functionality contained within Storage Connect.

### Objective 2: Implement an Azure-based backend SQL database
as a choice when defining system setup. That is, either an on premise database can be used or a cloud-based one.

### Objective 3: Mobile client side changes
At the moment, Adrian Harwood has a .Net library he wrote to make it easy to write applications that want to use the Storage Connect web service. It essentially encapsulates all the JSON and API calls making it quick and intuitive to add this capability to an app without having to write all the HTTP requests out within the application. If we add some new functionality to Storage Connect, change the API or change the protocol we will need to upgrade this library as well to ensure it remains compatible.

### Objective 4: Learning outcomes
i.e. document what we did.

### Constraints
The RSE developer of Storage Connect is not available for the May sprint days. The .Net API deverloper could make days 2 and 3. It may, therefore, be better to leave for a subsequent event.
