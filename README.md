# IdentityServer4
+ https://docs.identityserver.io/en/latest/index.html

# IdentityServer4 + ReactJS + ASP.NET Core 5 Web API
+ **C**: https://github.com/workcontrolgit/react-oidc-client-js (based on https://github.com/skoruba/react-oidc-client-js.git)
+ **A**: https://github.com/workcontrolgit/catnetcoreapi
+ **T**: https://github.com/workcontrolgit/TokenProject.AdminUI

# ASP.NET Core Security
+ https://docs.microsoft.com/en-us/aspnet/core/security/?view=aspnetcore-5.0
+ ASP.NET Core 5
+ ASP.NET Core Identity
+ OpenIdConnect with IdentityServer4
+ OAuth2 with IdentityServer4

# IdentityServer4 Admin UI version 2.0.1
+ https://github.com/skoruba/IdentityServer4.Admin
+ https://blog.bitscry.com/2020/02/07/identityserver4-management-using-skoruba-identityserver4-admin/
+ https://gitter.im/skoruba/IdentityServer4.Admin
+ https://github.com/workcontrolgit/TokenProject.AdminUI
  + https://www.youtube.com/watch?v=11LpCjXuUgA
  + https://www.youtube.com/watch?v=m_EEpPTCthM

# Videos:
+ https://www.youtube.com/watch?v=bw5hnMNlD6s (Part 1)
+ https://www.youtube.com/watch?v=EOy1ch_g6uk (Part 2)
+ https://www.youtube.com/watch?v=4JppmIxadbc (Part 3) (SSO and SAML 2.0)

# OAuth2
+ https://oauth.net/2/oauth-best-practice/

# AAD
+ https://github.com/AzureAD/azure-activedirectory-identitymodel-extensions-for-dotnet

## IdentityServer4 supports a variety of client connections
+ **PKCE flow** - for Mobile, SPA application connection
+ **Combined flow** - for Server-side Web application connections
+ **Resource owner password stream** - for Machine/Robot application connection
+ **Client authentication information flow** - for Server-to-Server application connections
+ **Device flow** - for Limited Input Device application connections

## Install Tools
+ Windows 10
+ Docker Desktop 3.5.2 (665001)
+ Visual Studio 2019 Community
  + .NET Core 5.0 SDK
+ NodeJS
+ Git and Git for Windows
+ SQL Server Express LocalDB

## Install Skoruba.IdentityServer4.Admin.Templates
+ dotnet new -i Skoruba.IdentityServer4.Admin.Templates::2.0.1

## Create new solution
+ Create new solution
  + md C:\IdSrv4\IdSrv4Admin\
  + cd C:\IdSrv4\IdSrv4Admin\
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
