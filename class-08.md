## Article - *A Brief History of Local Storage*

* Cookies originally held data - downside: only hold 4k of data, unencrypted, slow down application
* `userData` stores up to 64kb of data
* Flash cookies stored up to 100kb of data (2002)
* Google created Gears - open source browser plugin (2006)
* `dojox.storage` unified Adobe, Flash, Gears, Adobe AIR, & early HTML5 (2009)
* All solutions were specific to single browser or thrid-party plugin

* HTML5 Storage - local storage or DOM storage - `localStorage`
    * store key-value pairs locally on client web browser
    * never transmitted to remote web server
    * implemented natively by web browser

    * `if (Modernizr.localstorage) {
  // window.localStorage is available!
} else {
  // no native support for HTML5 storage :(
  // maybe try dojox.storage or a third-party solution
}`

    * Data stored as string 
    * `getItem()` `setItem()`
    * `var foo = localStorage.getItem("bar");
// ...
localStorage.setItem("bar", foo);` - can be written as - `var foo = localStorage["bar"];
// ...
localStorage["bar"] = foo;`

    * to remove storage - `removeItem(in DOMString key);
  void clear();
};`

    * get total number of values in storage - `readonly attribute unsigned long length;
  getter DOMString key(in unsigned long index);`

    * to track changes - set event `if (window.addEventListener) {
  window.addEventListener("storage", handle_storage, false);
} else {
  window.attachEvent("onstorage", handle_storage);
};`
        * to callback (e = storage event object) - `function handle_storage(e) {
  if (!e) { e = window.event; }
}`

    * storage limited to 5MB
     