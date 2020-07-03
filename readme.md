# CompileTimeApiClient
Using NSwag and dotnet tooling to generate an api client on build.
Includes a deployment script to pack the client as a NuGet, with auto incrementing version numbers.

## /ApiClientGeneration/Candy.Api/
A default api, with NSwag.AspNetCore configured.

## /ApiClientGeneration/Candy.Api.Clients/
A class library with a pre-build target to generate the nswag client when building.

## /deploy/
An Azure DevOps deployment script that builds the api and packs the client into a nuget with an automatically incrementing version number.
