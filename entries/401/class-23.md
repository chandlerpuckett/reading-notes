# Room
> Room provides an abstraction layer over SQLite to allow fluent database access while harnessing the full power of SQLite

- Apps that handle non-trivial amounts of structured data can benefit greatly from persisting that data locally


#### There are 3 major components in Room:
1. Database
    - Contains the database holder and serves as the main access point for the underlying connection to your app's persisted, relational data
      - Be an abstract class that extends `RoomDatabase`
      - Include the list of entities associated with the database within the annotation
      - Contain an abstract method that has 0 arguments and returns the class that is annotated with `@Dao`
2. Entity
    - Represents a table within the database
3. DAO
    - Contains the methods used for accessing the database

# Defining Data using Room Entities
> When using the Room persistence library, you define sets of related fields as entities. For each entity, a table is created within the associated `Database` object to hold the items. You must reference the entity class through the `entities` array in the `Database` class

- To persist a field, Room must have access to it

### Use a primary key
### Ignore fields
### Provide table search support
### Include AutoValue-based objects