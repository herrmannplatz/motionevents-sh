# jQuery Motion Events Plugin

Shorthands for transtionend and animationend events.

Usage
------

You can subscribe to 'transtionend', 'animationstart', 'animationiteration' and 'animationend' events by calling a function with the same name on your jquery element.

NOTE: Return `true` will dispose the event subscription.

```javascript
$('div').transitionend(function(e) {
  // do some stuff
  return true;
});

To listen to a specific transition e.g. when using multiple properties

```javascript
$('div').transitionend({
  opacity: function(e) {
    // do some stuff
    return true;
  },
  color: function(e) {
    // do some stuff
    return true;
  }
});