#Download Any Microservice from GitHub or use One of the Following for Demo

1. Visit https://github.com/rajib2github/pitshop-microservices/ to view PitShop Microservice
if You want to run pitshop  execute following
`git clone  https://github.com/rajib2github/pitshop-microservices`{{execute}}
This tutorial is based on Pitshop only


2. https://github.com/suadev/dotnet-istanbul-microservices-demo Another Event Driven Microservice
if You want to run Product  execute following
`git clone  https://github.com/suadev/dotnet-istanbul-microservices-demo`{{execute}}

3. Vist https://github.com/dockersamples/example-voting-app for Voting App 
if You want to run Voting app  execute following
`git clone  https://github.com/dockersamples/example-voting-app`{{execute}}


4. Visit https://github.com/dotnet-architecture/eShopOnContainers to view MS Eshop Container source
if You want to run eShoponContainers  execute following
`git clone  https://github.com/dotnet-architecture/eShopOnContainers`{{execute}}

Verify source course is downloaded . IDE will pickup the changes.


Goto Pitshop-Microservice\src
Open Docker-compose.yml file 
Search for microsoft/mssql-server-linux:latest (line 17)
Replace with  justin2004/mssql_server_tiny

mssqlserver some reason looking for 2GB memory space. Otherwise it fails. Local machine it is easy to increase the memory
Unix mssql_server_tiny image is a wrapper around SQLServer docker ignores 2GB check. More about this 
https://github.com/justin2004/mssql_server_tiny

Issue is discussed here.
https://github.com/Microsoft/mssql-docker/issues/114
