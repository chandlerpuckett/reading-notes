# Spring Boot & Oauth

There are several samples building on each other, adding new features at each step:

**simple**: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).

**click**: adds an explicit link that the user has to click to login.

**logout**: adds a logout link as well for authenticated users.

**two-providers**: adds a second login provider so the user can choose on the home page which one to use.

**custom-error**: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API.

### Add a Home Page
In your new project, create `index.html` in the `src/main/resources/static` folder. You should add some stylesheets and JavaScript links so the result looks like this:


## Request Mapping Shortcuts
Spring Framework 4.3 introduced a few new HTTP mapping annotations, all based on @RequestMapping:

- @GetMapping
- @PostMapping
- @PutMapping
- @DeleteMapping
- @PatchMapping

## Comparing Repositories
typical CRUD functionality:

- `save(…)` – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
- `findOne(…)` – get a single entity based on passed primary key value
- `findAll()` – get an Iterable of all available entities in database
- `count()` – return the count of total entities in a table
- `delete(…)` – delete an entity based on the passed object
- `exists(…)` – verify if an entity exists based on the passed primary key value

> When using Pageable, we create a Pageable object with certain properties and we've to specify at least:

1. Page size
2. Current page number
3. Sorting
