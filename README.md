# IdentityServer4 Admin UI version 2.0.1

## Install Tools
+ Windows 10
+ Docker Desktop 3.5.2 (665001)
+ Visual Studio 2019 Community
+ NodeJS
+ Git and Git for Windows
+ SQL Server Express LocalDB

## Install Skoruba.IdentityServer4.Admin.Templates
+ dotnet new -i Skoruba.IdentityServer4.Admin.Templates::2.0.1

## Create new solution
+ Create new solution
  + dotnet new skoruba.is4admin --name Identity --title Identity --adminemail "admin@kenken.com" --adminpassword "Abc@123$" --adminrole Admin --adminclientid ClientId --adminclientsecret "Abc@123$" --dockersupport true
+ Creat new DB in SQL Server Express LocalDB
+ Change connection string
+ Build success solution
  + cd C:\IdSrv4\IdSrv4Admin\**Identity\src\Identity.STS.Identity**
  + npm install
+ Set multiple startup projects
  + Identity.Admin
  + Identity.Admin.Api  
  + Identity.STS.Identity
+ F5 to run solution
