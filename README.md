# orgm-DemoMicroServicesProject
This is a Demo Microservices .Net Project with databases and Docker Compose.
There are 5 projects(microservices) in the solution; Blazor web server UI, Ocelot API Gateway, Customer Web API, Product Web API & Order Web API.
The customer web API & Product web API are connectted to a MySql Databases on different ports.
The Order web API is connected to a MongoDB database.
The UI communicates only with the Ocelot API gateway.
The API gateway communicates with the Web APIs which communicates with the various databases.
The UI is used for CRUD operations which is sent to the database.
The Docker Compose Ochestrates how the communication happens & how the ports are exposed & communicate.
At runtime, the Order page is dependent on the Customer & Product page because thats what will be used to make an Order.
Each Project has a Dockerfile which tells the sevice has to run.
