Usage
=====

Init
----

Pick a wrapper, run init, and voila!

```javascript
jQuery("#wrapper").slideto('init');
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
```
Currently, the 'next' method does not support looping. The 'prev' method does, however. I blame the mysterious design of jQuery.eq()