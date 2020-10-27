# Serverless
> Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers

- A serverless application runs in stateless compute containers that are event-triggered

#### Cloud Services:
1. AWS Lambda
2. Google Cloud Functions
3. Azure Functions
4. IBM OpenWhisk
5. Alibaba Function Compute
6. Iron Functions
7. Auth0 Webtask
8. Oracle Fn Project
9. Kubeless

**Pricing**
One of the major advantages of using Serverless is reduced cost, for years the cost of provisioning servers and maintaining that 24x7 server team which blew a hole in your pocket is gone

**Networking**
The downside is that Serverless functions are accessed only as private APIs

**3rd Party Dependencies**
Most, if not all of your projects have external dependencies, they rely on libraries that are not built into the language or framework you use. You often use libraries with functionality that includes cryptography, image processing, etc., these libraries can be pretty heavy. Without system-level access, you must package these dependencies into the application itself

### The Serverless App
1. **Client Application**
  - UI is rendered client side in Modern Frontend Javascript App which allows us to use a simple, static web server
2. **Web Server**
  - Amazon S3 provides a robust and simple web server. All of the static HTML, CSS and JS files for our application can be served from S3
3. **Lambda Functions (FaaS)**
  - They are the key enablers in Serverless architecture. Some popular examples of FaaS are AWS Lambda, Google Cloud Functions and Microsoft Azure Functions
4. **Security Token Service (STS)**
  - generates temporary AWS credentials (API key and secret key) for users of the application. These temporary credentials are used by the client application to invoke the AWS API (and thus invoke Lambda)
5. **User Authentication**
  - WS Cognito is an identity service which is integrated with AWS Lambda. With Amazon Cognito, you can easily add user sign-up and sign-in to your mobile and web apps
6. **Database**
  - AWS DynamoDB provides a fully managed NoSQL database. DynamoDB is not essential for a serverless application but is used as an example here