# Intent Filters

[Intent Filters Documentation](https://developer.android.com/training/basics/intents/filters)

### Allowing Other Apps to Start Your Activity

- if you're building an app that supports share functions, it should support the `ACTION_SEND` intent

> To allow other apps to start your activity in this way, you need to add an `<intent-filter>` element in your manifest file for the corresponding `<activity>`element

When an app calls `startActivity()` or `startActivityForResult()`, with an implicit intent, the system finds which activity (or activities) can respond to the intent

### Adding Intent Filters


**Action**

- `ACTION_SEND`
- `ACTION_VIEW`

**Data**
- intent filter goes in the `data` element
- specify the MIME type

**Category**
- all implicit intents are defined with `CATEGORY_DEFAULT` by default