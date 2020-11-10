# Location

[Location Retrieve](https://developer.android.com/training/location/retrieve-current)

> Using the Google Play services location APIs, your app can request the last known location of the user's device. In most cases, you are interested in the user's current location, which is usually equivalent to the last known location of the device

- uses fused location provider

**Set Up Google Play Services**
- required for the fused location provider

**Specify App Permissions**
**Create location services client**
- `onCreate()` create an instance of the fused location provider
- `getLastLocation()` used to retrieve the device location
  - this returns a `Task` with a `Location` object with latitude and longitude coordinates of a geographic location

**Maintain a current best estimate**
- check whether the location retrieved is significantly newer than previously fetched location
- check whether the accuracy claimed by the location is better or worse than that of the previous estimate
- Check the provider that's associated with the new location. Decide whether you trust this provider more than the one used in your app's cached location

