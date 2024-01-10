# EFCrud - the C# library for the EmployeeEFCrud


- API version: 1.0
- SDK version: 1.0.8
- Build package: org.openapitools.codegen.languages.CSharpClientCodegen

<a id="frameworks-supported"></a>
## Frameworks supported

## .NET Compatibility

| Version | Compatibility |
|---------|---------------|
| .NET 5.0 | `net5.0`, `net5.0-windows` |
| .NET 6.0 | `net6.0`, `net6.0-android`, `net6.0-ios`, `net6.0-maccatalyst`, `net6.0-macos`, `net6.0-tvos`, `net6.0-windows` |
| .NET 7.0 | `net7.0`, `net7.0-android`, `net7.0-ios`, `net7.0-maccatalyst`, `net7.0-macos`, `net7.0-tvos`, `net7.0-windows` |
| .NET 8.0 | `net8.0`, `net8.0-android`, `net8.0-ios`, `net8.0-maccatalyst`, `net8.0-macos`, `net8.0-tvos`, `net8.0-windows` |

## .NET Core Compatibility

| Version | Compatibility |
|---------|---------------|
| .NET Core 3.1 | `netcoreapp3.1` |


## Dependencies

- [RestSharp](https://www.nuget.org/packages/RestSharp) - 106.13.0 or later
- [Json.NET](https://www.nuget.org/packages/Newtonsoft.Json/) - 13.0.2 or later
- [JsonSubTypes](https://www.nuget.org/packages/JsonSubTypes/) - 1.8.0 or later
- [System.ComponentModel.Annotations](https://www.nuget.org/packages/System.ComponentModel.Annotations) - 5.0.0 or later

The DLLs included in the package may not be the latest version. We recommend using [NuGet](https://docs.nuget.org/consume/installing-nuget) to obtain the latest version of the packages:
```
Install-Package RestSharp
Install-Package Newtonsoft.Json
Install-Package JsonSubTypes
Install-Package System.ComponentModel.Annotations
```

NOTE: RestSharp versions greater than 105.1.0 have a bug which causes file uploads to fail. See [RestSharp#742](https://github.com/restsharp/RestSharp/issues/742).
NOTE: RestSharp for .Net Core creates a new socket for each api call, which can lead to a socket exhaustion problem. See [RestSharp#1406](https://github.com/restsharp/RestSharp/issues/1406).

<a id="installation"></a>
## Installation
Run the following command to generate the DLL
- [Mac/Linux] `/bin/sh build.sh`
- [Windows] `build.bat`

Then include the DLL (under the `bin` folder) in the C# project, and use the namespaces:
```csharp
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;
```
<a id="packaging"></a>
## Packaging

A `.nuspec` is included with the project. You can follow the Nuget quickstart to [create](https://docs.microsoft.com/en-us/nuget/quickstart/create-and-publish-a-package#create-the-package) and [publish](https://docs.microsoft.com/en-us/nuget/quickstart/create-and-publish-a-package#publish-the-package) packages.

This `.nuspec` uses placeholders from the `.csproj`, so build the `.csproj` directly:

```
nuget pack -Build -OutputDirectory out EFCrud.csproj
```

Then, publish to a [local feed](https://docs.microsoft.com/en-us/nuget/hosting-packages/local-feeds) or [other host](https://docs.microsoft.com/en-us/nuget/hosting-packages/overview) and consume the new package via Nuget as usual.

<a id="usage"></a>
## Usage

To use the API client with a HTTP proxy, setup a `System.Net.WebProxy`
```csharp
Configuration c = new Configuration();
System.Net.WebProxy webProxy = new System.Net.WebProxy("http://myProxyUrl:80/");
webProxy.Credentials = System.Net.CredentialCache.DefaultCredentials;
c.Proxy = webProxy;
```

<a id="getting-started"></a>
## Getting Started

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using EFCrud.Api;
using EFCrud.Client;
using EFCrud.Model;

namespace Example
{
    public class Example
    {
        public static void Main()
        {

            Configuration config = new Configuration();
            config.BasePath = "https://localhost:7217";
            var apiInstance = new AuthApi(config);
            var userdto = new Userdto?(); // Userdto? |  (optional) 

            try
            {
                User result = apiInstance.ApiAuthLoginPost(userdto);
                Debug.WriteLine(result);
            }
            catch (ApiException e)
            {
                Debug.Print("Exception when calling AuthApi.ApiAuthLoginPost: " + e.Message );
                Debug.Print("Status Code: "+ e.ErrorCode);
                Debug.Print(e.StackTrace);
            }

        }
    }
}
```

<a id="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *https://localhost:7217*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AuthApi* | [**ApiAuthLoginPost**](docs/AuthApi.md#apiauthloginpost) | **POST** /api/Auth/login | 
*AuthApi* | [**ApiAuthRegisterPost**](docs/AuthApi.md#apiauthregisterpost) | **POST** /api/Auth/register | 
*EmployeesApi* | [**ApiEmployeesGet**](docs/EmployeesApi.md#apiemployeesget) | **GET** /api/Employees | 
*EmployeesApi* | [**ApiEmployeesIdDelete**](docs/EmployeesApi.md#apiemployeesiddelete) | **DELETE** /api/Employees/{id} | 
*EmployeesApi* | [**ApiEmployeesIdGet**](docs/EmployeesApi.md#apiemployeesidget) | **GET** /api/Employees/{id} | 
*EmployeesApi* | [**ApiEmployeesIdPut**](docs/EmployeesApi.md#apiemployeesidput) | **PUT** /api/Employees/{id} | 
*EmployeesApi* | [**ApiEmployeesPost**](docs/EmployeesApi.md#apiemployeespost) | **POST** /api/Employees | 
*FeaturesApi* | [**ApiFeaturesIdDelete**](docs/FeaturesApi.md#apifeaturesiddelete) | **DELETE** /api/Features/{id} | 
*FeaturesApi* | [**ApiFeaturesIdPut**](docs/FeaturesApi.md#apifeaturesidput) | **PUT** /api/Features/{id} | 
*RolesApi* | [**ApiRolesAddEmployeeRolePost**](docs/RolesApi.md#apirolesaddemployeerolepost) | **POST** /api/Roles/Add-EmployeeRole | 
*RolesApi* | [**ApiRolesAddRolesPost**](docs/RolesApi.md#apirolesaddrolespost) | **POST** /api/Roles/Add-roles | 
*RolesApi* | [**ApiRolesDeleteEmpRoleDelete**](docs/RolesApi.md#apirolesdeleteemproledelete) | **DELETE** /api/Roles/Delete-EmpRole | 
*RolesApi* | [**ApiRolesShowEmployeeRolesGet**](docs/RolesApi.md#apirolesshowemployeerolesget) | **GET** /api/Roles/Show-EmployeeRoles | 
*RolesApi* | [**ApiRolesShowRolesGet**](docs/RolesApi.md#apirolesshowrolesget) | **GET** /api/Roles/Show-roles | 


<a id="documentation-for-models"></a>
## Documentation for Models

 - [Model.Employee](docs/Employee.md)
 - [Model.Roles](docs/Roles.md)
 - [Model.User](docs/User.md)
 - [Model.UserRoles](docs/UserRoles.md)
 - [Model.Userdto](docs/Userdto.md)


<a id="documentation-for-authorization"></a>
## Documentation for Authorization


Authentication schemes defined for the API:
<a id="oauth2"></a>
### oauth2

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header

