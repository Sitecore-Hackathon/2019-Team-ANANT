# Documentation


## Summary

Team ANANT chose the xConnect and Universal Tracker category because it combines two of our company's practices : Customer Experience & Data Analytics.  We seek to answer the question of "What is my customer experience doing around the globe in real time?" Currently, there are limited real-time planet scale options for storage when it comes to Sitecore xConnect.  The top two most used options are MongoDB and SQL Server.  MongoDB has very limited scale or real-time analytical streaming options of which more and more companies are choosing to move away from the product and use SQL Server.  SQL Server is very new to noSQL analytical storage and only scales well in the cloud.  It also has few real-time analytical streaming options ( such as data graphing or the ability to see page views in real time around the globe).  

Sitecore has plans to implement Azure CosmosDB as an xConnect storage option, however there is no official connector for xConnect and some customers wish to get a head start on the analytical platforms of the future.  We chose to use the Free Azure CosmosDB Emulator in our demo so customers can create proof of concepts of their analytical engines at Azure.  Once customers are comfortable, they can simply setup Azure CosmosDB and switch the connection strings.

**Category:** Best use of xConnect and/or Universal Tracker

The purpose of our module is to illustrate ways in which real-time hybrid cloud options can be added to xConnect.  xConnect is a powerful concept but presents very few options ( mainly 2 ) when it comes to analytical storage.  This can limit IT teams and Data Teams in their pursuit of learning what the user is doing in real time between clouds.  In many cases, it can be extremely expensive to support scaled out MongoDB or planet scaled SQL Server on Azure or AWS.  Our solution presents the ability to get started with Microsoft's true Planet Scale Real-Time Database.  Customers can preview how their Sitecore Installations would hold up on Azure plus take advantage of CosmosDB's advanced data operations.
 

## Pre-requisites

Does your module rely on other Sitecore modules or frameworks?

- xConnect is required as it is the API for Analytics 
- Experience Analytics must be turned on
- Azure CosmosDB Emulator

## Installation

Provide detailed instructions on how to install the module, and include screenshots where necessary.

1. Use the Sitecore 9.1 Installation wizard to install Sitecore [package](https://dev.sitecore.net/Downloads/Sitecore_Experience_Platform/91/Sitecore_Experience_Platform_91_Initial_Release.aspx)
2. Create some pages in your Sitecore Installation 
3. Enable Experience Analytics
4. [Docker](https://hub.docker.com/r/microsoft/azure-cosmosdb-emulator/) up the Latest Version of Azure CosmosDB Emulator or install manually here [package](https://aka.ms/cosmosdb-emulator)
5. Enable the MongoDB Sitecore xConnect Connector
6. Enable the MongoDB Azure CosmosDB emulator and obtain it's connecting string from the Local Azure Emulator Portal 
7. Update the MongoDB xConnect Connection String to point to your Azure CosmosDB Emulator MongoDB URL
8. Browse the pages on your Sitecore Site to create Analytical data
9. Confirm data is being stored in the Azure CosmosDB Emulator using the Emulator Portal
10.Confirm that the Experience Analytics Dashboard behaves as expected insdie of Sitecore

## Configuration

The xConnect MongoDB Configuration needs to be updated in order to talk to Azure CosmosDB.  You simply enable the MongoDB Configuration file and update its connection string with the Azure CosmosDB MongoDB Connection string.


## Usage

1. Our module is to be used as an example to quickly create a proof of concept around Sitecore and Azure CosmosDB xDB integration.
2. Customers can be up in within hours testing real time queries that can be transfered to the full Azure Cosmos
3. Customers can create queries based of Sitecore User Experience metrics such as Page Views, Bounce Rate, etc not to mention custom metrics and track them in real time.

