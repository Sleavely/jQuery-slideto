Usage
=====

Init
----

Pick a wrapper, run init, and voila!

```javascript
jQuery("#wrapper").slideto('init');

//or, with options
jQuery("#wrapper").slideto('init', {
  //element to show at first
  offset: 0,
  //css property for #wrapper
  overflow: "hidden"
});
```

Sliding
-------

Though, in all honesty, you probably need some more code. To make things move:

```javascript
//if you know where you are going
jQuery("#some-child-of-the-wrapper").slideto();

//and if you dont
jQuery("#wrapper").slideto('next');
jQuery("#wrapper").slideto('prev');

//With options:
jQuery("#some-child-of-the-wrapper").slideto({
  instant: false, //animate movement or just css it
  speed: "fast"
});
//these options can be passed as a secondary parameter to the 'next' and 'prev' methods too
```
Currently, the 'next' method does not support looping. The 'prev' method does, however. I blame the mysterious design of jQuery.eq()