# Spring Request Mapping

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
