# Espresso Testing
> Espresso tests state expectations, interactions, and assertions clearly without the distraction of boilerplate content, custom infrastructure, or messy implementation details getting in the way

- Espresso is targeted at developers, who believe that automated testing is an integral part of the development lifecycle

- While it can be used for black-box testing, Espresso’s full power is unlocked by those who are familiar with the codebase under test

- Each time your test invokes `onView()`, Espresso waits to perform the corresponding UI action or assertion until the following synchronization conditions are met

## Packages

- `espresso-core` - Contains core and basic View matchers, actions, and assertions. See Basics and Recipes.
- `espresso-web` - Contains resources for WebView support.
- `espresso-idling-resource` - Espresso's mechanism for synchronization with background jobs.
- `espresso-contrib` - External contributions that contain DatePicker, RecyclerView and Drawer actions, accessibility checks, and CountingIdlingResource.
- `espresso-intents` - Extension to validate and stub intents for hermetic testing.
- `espresso-remote` - Location of Espresso's multi-process functionality.

#### The Espresso Test Recorder tool lets you create UI tests for your app without writing any test code

> Before using Espresso Test Recorder, **make sure you turn off animations**

#### Add assertions to verify UI elements

- `text is`: Checks the text content of the selected View element
- `exists`: Checks that the View element is present in the current View hierarchy visible on the screen
- `does not exist`: Checks that the View element is not present in the current View hierarchy