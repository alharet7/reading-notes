# Entity Framework and APIs 

Entity Framework and Web API are powerful tools that can help us create data-driven web applications with .NET. Entity Framework simplifies the data access layer by abstracting the database operations and mapping them to objects. Web API enables us to expose our data and business logic as RESTful services that can be consumed by various clients. By combining Entity Framework and Web API, we can build modern, scalable, and secure web applications that leverage the best of both worlds.

---

## Data Seeding:

Data seeding is the process of populating a database with an initial set of data.

There are several ways this can be accomplished in EF Core:

- Model seed data
- Manual migration customization
- Custom initialization logic


Model seed data is a way of associating seed data with an entity type as part of the model configuration. Then EF Core migrations can automatically compute what insert, update or delete operations need to be applied when upgrading the database to a new version of the model.

Manual migration customization is a way of modifying the generated migration code to include seed data operations. This gives you more control over how the seed data is applied, but it also requires more manual work.

Custom initialization logic is a way of writing your own code to seed the database, either by using the DbContext API or by executing SQL commands. This gives you the most flexibility, but it also means you have to handle the logic of checking and updating the seed data yourself.

---

## User secrets:

User secrets is a secure way of storing private user information such as API keys, client secrets, and connection strings. Essentially anything that you don’t want others to know about when using your code base.

The user secrets is not uploaded to any source control. This ensures your keys do in fact stay “secret” to your local machine.

