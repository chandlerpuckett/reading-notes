# CHEATSHEET

`localStorage.setItem("x", foo);`

var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);

interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};

- Calling `removeItem()` with a non-existent key will do nothing.


property to get the total number of values in the storage area, and to iterate through all of the keys by index (to get the name of each key):

interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};

- If you want to keep track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.


> if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};

The handle_storage callback function will be called with a StorageEvent object, except in Internet Explorer where the event object is stored in window.event.

function handle_storage(e) {
  if (!e) { e = window.event; }
}

- key
- oldValue
- newValue
- url

- 5 mb storage
- you’re storing strings, not data in its original format

> Data is stored as strings. If you are storing something other than a string, you’ll need to coerce it yourself when you retrieve it



[home](https://chandlerpuckett.github.io/reading-notes)

