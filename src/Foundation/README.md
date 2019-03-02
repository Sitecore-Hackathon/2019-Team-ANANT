# Source Code : Foundation

Add your source code for your Foundation in this folder.


Powershell script to install Azure Cosmo DB Emulator

$client = new-object System.Net.WebClient
$client.DownloadFile("https://cosmosdbportalstorage.azureedge.net/emulator/2019_02_28_2.2.1-2b4af9b3/azure-cosmosdb-emulator-2.2.1-2b4af9b3.msi","C:\Sitecore\azure-cosmosdb-emulator-2.2.1-2b4af9b3.msi")
$exitCode = (Start-Process "msiexec.exe" -ArgumentList "/i C:\Sitecore\azure-cosmosdb-emulator-2.2.1-2b4af9b3.msi","/qb!" -wait -passthru).ExitCode
