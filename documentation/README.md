# Documentation


## Summary

Team ANANT chose the xConnect and Universal Tracker category because it combines two of our company's practices : Customer Experience & Data Analytics.  We seek to answer the question of "What is my customer experience doing around the globe in real time?" Currently, there are limited real-time planet scale options for storage when it comes to Sitecore xConnect.  The top two most used options are MongoDB and SQL Server.  MongoDB has very limited scale or real-time analytical streaming options of which more and more companies are choosing to move away from the product and use SQL Server.  SQL Server is very new to noSQL analytical storage and only scales well in the cloud.  It also has few real-time analytical streaming options ( such as data graphing or the ability to see page views in real time around the globe).  Sitecore has plans to implement Azure CosmosDB as an xConnect storage option, however this requires a customer to have and pay for Azure when customers might decide they want a hybrid cloud or another cloud vendor.  And as mention, these are only plans, there is no code for xConnect on CosmosDB.

Enter UserGrid.  User Grid allows companies to manage and create applications on top of a scaled "backend-as-a-service".  UserGrid can be used to scale more things than simply analytics but for this hackathon we are using it to scale Cassandra.  UserGrid is a stack of tools that uses Cassandra to store data.  UserGrid has the ability to emulate a MongoDB connection and store the data in a global hybrid open source database ( or any database) like cassandra.  This way customers can scale their analytics on premise or in the cloud and have real-time streaming combined with advanced data operations.

**Category:** Best use of xConnect and/or Universal Tracker

The purpose of our module is to illustrate ways in which real-time hybrid cloud options can be added to xConnect.  xConnect is a powerful concept but presents very few options ( mainly 2 ) when it comes to analytical storage.  This can limit IT teams and Data Teams in their pursuit of learning what the user is doing in real time between clouds.  In many cases, it can be extremely expensive to support scaled out MongoDB or planet scaled SQL Server on Azure or AWS.  Our solution presents the best of both worlds by integrating the UserGrid layer to handle analytical operations.  As technology changes, different options can be swapped in but Sitecore is simply using xConnect to talk to UserGrid for all analytical information.  In theory, its technology agnostic. 
 

## Pre-requisites

Does your module rely on other Sitecore modules or frameworks?

- xConnect is required as it is the API for Analytics 
- Experience Analytics must be turned on
- UserGrid 2.1 or greater is preferred 

## Installation

Provide detailed instructions on how to install the module, and include screenshots where necessary.

1. Use the Sitecore 9.1 Installation wizard to install Sitecore [package](https://dev.sitecore.net/Downloads/Sitecore_Experience_Platform/91/Sitecore_Experience_Platform_91_Initial_Release.aspx)
2. Create some pages in your Sitecore Installation 
3. Enable Experience Analytics
4. Docker up the Latest Version of UserGrid
5. Enable the MongoDB Sitecore xConnect Connector
6. Enable the MongoDB UserGrid emulator 
7. Update the MongoDB xConnect Connection String to point to your UserGrid URL
8. Browse the pages on your Sitecore Site to create Analytical data
9. Confirm data is being stored in the UserGrid\Cassandra container of the UserGrid Stack

## Configuration

The xConnect MongoDB Configuration needs to be updated in order to talk to UserGrid.


## Usage

How does the end user use the Module?


## Video

Please provide a video highlighing your Hackathon module submission and provide a link to the video. Either a [direct link](https://www.youtube.com/watch?v=EpNhxW4pNKk) to the video, upload it to this documentation folder or maybe upload it to Youtube...

[![Sitecore Hackathon Video Embedding Alt Text](https://img.youtube.com/vi/EpNhxW4pNKk/0.jpg)](https://www.youtube.com/watch?v=EpNhxW4pNKk)
