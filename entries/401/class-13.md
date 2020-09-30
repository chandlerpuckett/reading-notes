# REST w/ Spring

### The data model 
- We must be careful to have different names for each association resource

### Creating the Associations
- **After persisting both instances, we can establish the relationship by using one of the association resources**

This is done using the HTTP method PUT, which supports a media type of text/uri-list, and a body containing the URI of the resource to bind to the association

To remove an association, we can call the endpoint with `DELETE` method

# Integration Testing
> Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system

First, any Spring enabled test will run with the help of `@RunWith(SpringJUnit4ClassRunner.class);` the runner is essentially the entry-point to start using the Spring Test framework
