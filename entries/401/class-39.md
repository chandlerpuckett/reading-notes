# Kinesis
> This sets up the AWS Analytics backend with Pinpoint and Kinesis

`amplify add analytics`

1. add the dependencies in your `build.gradle`
2. initialize by adding the plugins to your AWS configure try/catch
3. record events with `AnalyticsEvent` and call `Amplify.Analytics.recordEvent()`

- The Amplify analytics plugin records when an application opens and closes. This session information can be viewed either from your local computer’s terminal or the AWS Console for Pinpoint
> `amplify console analytics`

You can identify a users location by using `UserProfile.Location`

### Escape Hatch
> For advanced use cases where Amplify does not provide the functionality, you can retrieve the escape hatch to access the underlying Amazon Pinpoint client

