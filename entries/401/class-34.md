# Cognito
> The Amplify Auth category provides an interface for authenticating a user. Behind the scenes, it provides the necessary authorization to the other Amplify categories. It comes with default, built-in support for Amazon Cognito User Pool and Identity Pool. The Amplify CLI helps you to create and configure the auth category with an authentication provider

To start provisioning auth resources in the backend, go to your project directory and **execute the command**: `amplify add auth`

Enter the following when prompted:

? Do you want to use the default authentication and security configuration?
    `Default configuration`
? How do you want users to be able to sign in?
    `Username`
? Do you want to configure advanced settings?
    `No, I am done.`

When finished:
`amplify push`

### Install Amplify Libraries
Add the following dependency to your app‘s `build.gradle` along with others you added above in **Prerequisites** and click “Sync Now” when prompted
> `implementation 'com.amplifyframework:aws-auth-cognito:1.4.1'`

### Initialize Amplify Auth
- Add the Auth plugin along with any other plugins you added per the instructions in the Prerequisites section

> // Add this line, to include the **Auth plugin**.
`Amplify.addPlugin(new AWSCognitoAuthPlugin());`
`Amplify.configure(getApplicationContext());`

### Check the current Auth Session
- For testing purposes, you can run this from your MainActivity’s `onCreate` method

Amplify.Auth.fetchAuthSession ( <br>
  result -> Log.i("AmplifyQuickstart", result.toString()), <br>
  error -> Log.e("AmplifyQuickstart", error.toString()) <br>
);