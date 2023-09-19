# View components in ASP.NET Core

View components are similar to partial views, but they're much more powerful. View components don't use model binding, they depend on the data passed when calling the view component.

---

## A view component:

- Renders a chunk rather than a whole response.
- Includes the same separation-of-concerns and testability benefits found between a controller and view.
- Can have parameters and business logic.
- Is typically invoked from a layout page.

---

## A view component consists of two parts:

The class, typically derived from ViewComponent
The result it returns, typically a view.

- View components are intended anywhere reusable rendering logic that's too complex for a partial view, such as:
  - Dynamic navigation menus
  - Tag cloud, where it queries the database
  - Sign in panel
  - Shopping cart
  - Recently published articles
  - Sidebar content on a blog
  - A sign in panel that would be rendered on every page and show either the links to sign out or sign in, depending on the sign in state of the user.

