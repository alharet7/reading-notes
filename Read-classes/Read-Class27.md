# Views in ASP.NET Core MVC

Views in ASP.NET Core MVC are files that contain the HTML code and some special syntax to display the data from the model on the web page. Views are responsible for how the web page looks and interacts with the user. Views use a language called ***Razor***, which is a mix of ***HTML*** and ***C#***. Razor allows we to write code that can access the model data and generate dynamic ***HTML*** content.

Views are usually organized in folders that match the names of the controllers. For example, if we have a controller called ProductsController, we would have a folder called Products inside the Views folder, and inside that folder we would have the views for each action of the controller. This way, it is easy to find and maintain the views for each controller.

We can also use some features to make our views more reusable and consistent, such as:

- Layouts: These are views that contain common elements for all pages, such as header, footer, navigation menu, etc. We can specify a layout for our views and then only write the content that is specific to each page.

- Partial views: These are views that contain a piece of HTML code that can be used in multiple places. For example, we can have a partial view for a product card that shows the name, price, and image of a product. We can then use this partial view in different pages that need to display products.

- View components: These are classes that can generate HTML code and have some logic behind them. For example, we can have a view component for a shopping cart that shows the items, total price, and checkout button. We can then use this view component in any page that needs to show the shopping cart.

---

## Forms in .NET MVC

A form in .NET MVC is a way of creating web pages that can collect and submit data from the user to the server. A form in .NET MVC consists of three main components: the model, the view, and the controller.

- The **model** is a class that defines the properties and validation rules for the data that the form will handle. For example, if we want to create a form for a contact information, we can create a model class with properties like name, email, phone, etc. and add attributes to specify the data type, required fields, maximum length, etc.

- The **view** is a file that contains the **`HTML`** code and some special syntax to display the data from the model on the web page. The view uses a language called ***Razor***, which is a mix of **`HTML`** and **`C#`**. Razor allows we to write code that can access the model data and generate dynamic HTML content. We can use **tag helpers** or **HTML helpers** to create form elements like input, select, textarea, etc. and bind them to the model properties. We can also use validation helpers to display error messages if the data is invalid.

- The **controller** is a class that handles the user requests and performs actions on the model data. The controller has methods called **actions** that correspond to different ***HTTP*** verbs like **GET, POST, PUT, DELETE**, etc. WE can use attributes like [HttpGet] or [HttpPost] to specify which action should handle which request. We can also use parameters or model binding to receive the data from the form and pass it to the model or other services.

