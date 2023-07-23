# Navigation Properties and Routing

## Routing within MVC

 The ASP.NET Routing module is responsible for mapping incoming requests to particular MVC controller actions.

### Using the Default Route Table

ASP.NET Routing is setup in two places:

- enabled in the application's Web configuration file (Web.config file).
- a route table is created in the application's Global.asax file. The Global.asax file is a special file that contains event handlers for ASP.NET application lifecycle events.

## Routing within Core

Routing is responsible for matching incoming HTTP requests and dispatching those requests to the app's executable endpoints.Using endpoint information from the app, routing is also able to generate URLs that map to endpoints.

### Routing basics

Routing is registered in the middleware pipeline in `Startup.Configure`

Routing uses a pair of middleware:

- UseRouting adds route matching to the middleware pipeline.

- UseEndpoints adds endpoint execution to the middleware pipeline.

### ASP.NET Core endpoint definition

An ASP.NET Core endpoint is:

- Executable: Has a RequestDelegate.
- Extensible: Has a Metadata collection.
- Selectable: Optionally, has routing information.
- Enumerable: The collection of endpoints can be listed by retrieving the EndpointDataSource from DI.

### URL generation concept

Is the process by which routing can create a URL path based on a set of route values.

### Route constraint reference

Route constraints determine acceptable route values for routing requests and link generation by tokenizing URL paths and considering external data.
