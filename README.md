## Summary

Team ANANT chose the xConnect and Universal Tracker category because it combines two of our company's practices : Customer Experience & Data Analytics.  We seek to answer the question of "What is my customer experience doing around the globe in real time?" Currently, there are limited real-time planet scale options for storage when it comes to Sitecore xConnect.  The top two most used options are MongoDB and SQL Server.  MongoDB has very limited scale or real-time analytical streaming options of which more and more companies are choosing to move away from the product and use SQL Server.  SQL Server is very new to noSQL analytical storage and only scales well in the cloud.  It also has few real-time analytical streaming options ( such as data graphing or the ability to see page views in real time around the globe).  

Sitecore has plans to implement Azure CosmosDB as an xConnect storage option, however there is no official connector for xConnect and some customers wish to get a head start on the analytical platforms of the future.  We chose to use the Free Azure CosmosDB Emulator in our demo so customers can create proof of concepts of their analytical engines at Azure.  Once customers are comfortable, they can simply setup Azure CosmosDB and switch the connection strings.

**Category:** Best use of xConnect and/or Universal Tracker

The purpose of our module is to illustrate ways in which real-time hybrid cloud options can be added to xConnect.  xConnect is a powerful concept but presents very few options ( mainly 2 ) when it comes to analytical storage.  This can limit IT teams and Data Teams in their pursuit of learning what the user is doing in real time between clouds.  In many cases, it can be extremely expensive to support scaled out MongoDB or planet scaled SQL Server on Azure or AWS.  Our solution presents the ability to get started with Microsoft's true Planet Scale Real-Time Database.  Customers can preview how their Sitecore Installations would hold up on Azure plus take advantage of CosmosDB's advanced data operations.

## Screenshots

### Sitecore Experience Analytics Dashboard using Azure Cosmos DB for storage

![Sitecore Experience Analytics](documentation/images/im_sitecore_analytics.png?raw=true "Sitecore Analytics on CosmosDB")


### Sitecore Data Elements stored in Azure CosmosDB Collections 

![Sitecore Experience Analytics Collections](documentation/images/im_azure_sitecore_analytics.png?raw=true "Sitecore Collections")


### Sitecore Contact Collections 

![Sitecore Contact Collections](documentation/images/Im_sitecore_collections.png?raw=true "Sitecore Collections")

### Sitecore Contact Facet Collections 

![Sitecore Contact Facets Collections](documentation/images/im_sitecore_contact_facets.png?raw=true "Sitecore Collections")
