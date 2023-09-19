# View Components

View components offer the same separation of concerns and testability benefits as seen between a controller and a view.

A view component consists of two parts:

1. The class, derived from ViewComponent
2. The result it returns

## Writing A Simple View Component

- derive from the ViewComponent class,
- are decorated with the [ViewComponent] attribute, or
- have a name that ends with the "ViewComponent" suffix.

## Rendering a View Component

Within Razor views, we can use the `Component` helper and its `Invoke` method to render view components.

## Asynchronous View Components

 by using the `InvokeAsync` method  instead of an Invoke method, and return a `Task<IViewComponentResult>`.
