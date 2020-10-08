# Spring & Sockets

### import Spring Tool Suite (STS)

### Create a resource Representation Class

The service will accept messages that contain a name in a STOMP message whose body is a JSON object. If the name is `Fred`, the message might resemble the following:
`{
    "name": "Fred"
}`

- Upon receiving the message and extracting the name, the service will process it by creating a greeting and publishing that greeting on a separate queue to which the client is subscribed

- heavily relies on getters & setters

- Spring will use the Jackson JSON library to automatically marshal instances of type `Greeting` into JSON

### Create a message-handling controller

- In Spring’s approach to working with STOMP messaging, STOMP messages can be routed to `@Controller` classes. For example, the `GreetingController` (from `src/main/java/com/example/messagingstompwebsocket/GreetingController.java`)

1. The `@MessageMapping` annotation ensures that, if a message is sent to the `/hello` destination, the `greeting()` method is called
2. The payload of the message is bound to a `HelloMessage` object, which is passed into `greeting()`
3. Internally, the implementation of the method simulates a processing delay by causing the thread to sleep for one second. This is to demonstrate that, after the client sends a message, the server can take as long as it needs to asynchronously process the message. The client can continue with whatever work it needs to do without waiting for the response
4. After the one-second delay, the `greeting()` method creates a `Greeting` object and returns it. The return value is broadcast to all subscribers of `/topic/greetings`, as specified in the `@SendTo` annotation