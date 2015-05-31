# DataStorage
A library for web storage

##Use
>```javascript
var storage = new DataStorage({prefix:'baz'});    // set a custom prefix
storage.setItem("foo","bar");
storage.getItem("foo");                           // "bar"
storage.clear({key:"foo"});                       // clear only the specified key
storage.clear();                                  // clear all the keys
```
>```javascript
storage.setItem("foo",null);
test2.getItem("foo");                             // null
test2.getItem("b",{json:false});                  // "null"

