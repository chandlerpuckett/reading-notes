# Spring

- start with Spring Initializr
- In Spring’s approach to building web sites, HTTP requests are handled by a controller

### Spring Boot Devtools
**Spring Boot Devtools:**
- Enables hot swapping.
- Switches template engines to disable caching.
- Enables LiveReload to automatically refresh the browser.
- Other reasonable defaults based on development instead of production.

> The Spring Initializr creates an application class for you

The `main()` method uses Spring Boot’s `SpringApplication.run()` method to launch an application.

- You can run the application from the command line with Gradle or Maven

## Spring MVC & Thymeleaf

In a typical Spring MVC application, `@Controller` classes are responsible for preparing a model map with data and selecting a view to be rendered. This model map allows for the complete abstraction of the view technology and, in the case of Thymeleaf, it is transformed into a Thymeleaf context object (part of the Thymeleaf template execution context) that makes all the defined variables available to expressions executed in templates


