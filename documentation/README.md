# Documentation

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
4. Install the Azure CosmosDB Emulator using our Custom [PowerShell](https://github.com/Sitecore-Hackathon/2019-Team-ANANT/blob/master/src/Foundation/Install_Cosmos_Emu.ps1) or install manually here [package](https://aka.ms/cosmosdb-emulator)
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

