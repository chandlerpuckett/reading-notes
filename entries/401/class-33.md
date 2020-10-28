# GraphQL
> The `@connection` directive enables you to specify relationships between `@model` types. Currently, this supports one-to-one, one-to-many, and many-to-one relationships. You may implement many-to-many relationships using two one-to-many connections and a joining `@model` type

**Usage**
- Relationships between types are specified by annotating fields on an `@model` object type with the `@connection` directive.

**Has One**
- In the simplest case, you can define a one-to-one connection where a project has one team
- You can also define the field you would like to use for the connection by populating the first argument to the fields array and matching it to a field on the type

**Has Many**
- Note how a one-to-many connection needs an `@key` that allows comments to be queried by the `postID` and the connection uses this key to get all comments whose `postID` is the id of the post was called on. After it’s transformed, you can create comments and query the connected Post as follows

**Belongs To**
- You can make a connection bi-directional by adding a many-to-one connection to types that already have a one-to-many connection. In this case you add a connection from Comment to Post since each comment belongs to a post

**Many-to-many**
- You can implement many to many using two 1-M `@connections`, an `@key`, and a joining `@model`

### Limit
The default number of nested objects is 100. You can override this behavior by setting the `limit` argument

### Generates
In order to keep connection queries fast and efficient, the GraphQL transform manages global secondary indexes (GSIs) on the generated tables on your behalf. In the future you are investigating using adjacency lists along side GSIs for different use cases that are connection heavy
> Note After you have pushed a `@connection` directive you should not try to change it. If you try to change it, the DynamoDB UpdateTable operation will fail. Should you need to change a `@connection`, you should add a new `@connection` that implements the new access pattern, update your application to use the new `@connection`, and then delete the old `@connection` when it’s no longer needed

