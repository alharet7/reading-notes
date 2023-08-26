# Intro to MVC Submission Requirements

## Azure DevOps

Azure DevOps is a platform that provides several tools for better team collaboration. It supports a collaborative culture and set of processes that bring together developers, project managers, and contributors to develop software. It allows organizations to create and improve products at a faster pace than they can with traditional software development approaches. Azure DevOps provides integrated features that we can access through our web browser or IDE client. we can use all the services included with Azure DevOps, or choose just what we need to complement our existing workflows. Some of the services provided by Azure DevOps include Azure Boards, Azure Repos, Azure Pipelines, Azure Test Plans, and Azure Artifacts. we can work in the cloud using Azure DevOps Services or on-premises using Azure DevOps Server.

---

## MVC Basics

MVC stands for ***Model-View-Controller.*** It is an architectural/design pattern that separates an application into three main logical components: the Model, the View, and the Controller. Each of these components is built to handle specific development aspects of an application. The Model component corresponds to all the data-related logic that the user works with. The View component is used for all the UI logic of the application. The Controller acts as an interface between Model and View components to process all the business logic and incoming requests, manipulate data using the Model component and interact with the Views to render the final output. This separation of concerns allows for more efficient development and easier maintenance of applications.

MVC (Model-View-Controller) and traditional ASP.NET are two different approaches for building web applications, each with its own benefits:

**Separation of Concerns:**

- **Traditional ASP.NET:** The user interface (UI) and user actions are closely tied together in the same file (e.g., Sample.aspx and Sample.aspx.cs).
- **MVC:** The UI is separated from user actions. The View only handles UI, and user actions are defined in the Controller.

**Architecture:**

- **ASP.NET Web Application:** Follows a View-based architecture, which can be less efficient for action-based requirements.
- **MVC:** Follows an action-based architecture, where appropriate Views are displayed based on user actions. The code organization in MVC is cleaner and more organized.

**State Management:**

- **ASP.NET:** Uses View State to maintain the state of web pages, which can make pages heavy and inefficient due to frequent server trips.
- **MVC:** Does not rely on View State for state maintenance, leading to lighter and more efficient pages.

**Page Life Cycle:**

- **ASP.NET:** Has a detailed Page Life Cycle that adds to the response time of web pages, making them slower.
- **MVC:** Doesn't have a complex Page Life Cycle; requests directly hit the Controller, making response times faster.

**Testing:**

- **Traditional ASP.NET:** UI and business logic are tightly coupled, making testing challenging. Code-behind can't be tested separately.
- **MVC:** Promotes test-driven development by separating Models, Controllers, and Views. This allows for easier and more effective testing.

In summary, MVC offers better separation of concerns, a cleaner code structure, improved state management, faster response times, and enhanced testing capabilities compared to the traditional ASP.NET approach.

---

## Tag Helpers in ASP.NET Core

Tag Helpers in ASP.NET Core are server-side components that enable server-side code to participate in creating and rendering HTML elements in Razor files. They are used to perform defined transformations on HTML elements and can append a version number to the image name, for example. There are many built-in Tag Helpers for common tasks, such as creating forms, links, loading assets, and more. Tag Helpers are authored in C#, and they target HTML elements based on element name, attribute name, or parent tag. They provide an HTML-friendly development experience and a rich IntelliSense environment for creating HTML and Razor markup. Tag Helpers make developers more productive and able to produce more robust, reliable, and maintainable code using information only available on the server.

## Bootstrap

Bootstrap is a free front-end framework for faster and easier web development. It includes **`HTML`** and **`CSS`** based design templates for typography, forms, buttons, tables, navigation, modals, image carousels and many other components, as well as optional `JavaScript` plugins. Bootstrap also gives you the ability to easily create responsive designs. 
