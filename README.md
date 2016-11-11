# VaultBrowserSample_Forge_Demo
Vault Forge Demo that gets an Inventor Assembly from Vault and uploads it to a bucket

The .7z file has a Visual studio project that is an update to the VaultBrowser Sample in the Vault 2017 API SDK. The sample now does a read only access so you can remove this in the Post Build Events command line. (properties > Build Events tab)
xcopy "$(ProjectDir)..\..\..\..\bin\x64\clmloader.dll" "$(TargetDir)" /y 

clmloader.dll is needed for read access licensing in Vault 2017

You will need to change the code so that it logs into your vault. (the code that does this is in Form1.cs - search on "LogIn") 

The example uses three hard coded paths these are. They can be named anything but the code would need to be changed so the folders are found. 
C:\Vault_Forge_Local_Files  
C:\Vault_Forge_Local_Files_Copied  
C:\Vault_Forge_Local_Zip

The example uses Apprentice Server so you would need to have Inventor installed or Inventor View.

See the ForgeDemo.mp4 is a video demonstrating the use of this sample. 

