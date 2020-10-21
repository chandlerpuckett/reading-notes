# Recycler View
> If your app needs to display a scrolling list of elements based on large data sets (or data that frequently changes), you should use `RecyclerView`

#### The `RecyclerView` widget is a more advanced and flexible version of `ListView`.

- The views in the list are represented by *view holder* objects
- These objects are instances of a class you define by extending `RecyclerView`
- The view holder objects are managed by an adapter, which you create by extending `RecyclerView.Adapter`

### Add the support library
To access the `RecyclerView` widget, you need to add the v7 Support Libraries to your project as follows:
1. Open the `build.gradle` file for your app module.
2. Add the support library to the `dependencies` section

### Add RecyclerView to your layout
> Once you have added a RecyclerView widget to your layout, obtain a handle to the object, connect it to a layout manager, and attach an adapter for the data to be displayed