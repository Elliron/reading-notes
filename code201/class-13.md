# Local Storage
### Persistant local Storage
  - advantage over native client applications
  - OS has abstract layer for storing and retrieving application specific data
  - stored in registry, INI files, XML files or other platform convention
  - can embed your own database, invent your own file format, etc.

### Cookies
  - invented early in web history
  - can be used for persistent local storage 
  - included in every HTTP request
  - slows down data
  - sends data unencrypted over internet
  - limited to 4kb data

### Internet Explorer
  - Microsoft is tricksy, make us believe it was the only....
  - invented DTHML Behaviors
    - userData
      - allows web page to store up to 64 kb data
      - heirarchical XML based structure

### Flash
  - created in 2002
  - Adobe introduced Flash 6, misleading name of "Flash Cookies"
  - Local Shared Objects store up to 100 kb of data

### Gears
  - 2007 by Google
  - geolocation API in IE

# HTML 5 Storage
  - Web Storage
  - Web pages store named key/value pairs locally
  - Data never transmitted

### Check for storage

```
function supports_htrml5_storage() {
  try {
    return 'localStorage' in window && window['localStorage'] ~== null;
  } catch (e) {
    return false;
  }
}
```

- Modernizr

```
if (Modernizr.localstorage) {
} else {
}
```

### Using HTML 5 Storage

```
interface Storage {
  getter any getItem(in DOMString key);
  setter creator void setItem(in DOMString key, in any data);
};
```

``` 
var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);
```

``` var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;
```
```
interface Storage {
  deleter void removeItem(in DOMString key);
  void clear();
};
```

```
interface Storage {
  readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);
};
```

### Tracking changes

``` if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};
```

```
function handle_storage(e) {
  if (!e) {e = window.event; }
}
```

### Limitations in current browsers
- 5 mg storage space each origin gets by default

### Beyond

- Indeed Database API or "WebSimpleDB" or IndexedDB
  - exposed object store
  - object store shares concepts with SQL






[Home](../README.md)