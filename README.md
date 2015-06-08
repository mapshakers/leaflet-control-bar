leaflet-control-bar
=====================

Simple navigation bar for excellent javascript mapping library [Leaflet](http://leafletjs.com).

*Compatible with Leaflet 0.6.0 or newer*

## Example
[Check out demo!](http://filipzava.github.io/leaflet-control-bar)

## Using the plugin

### Usage
Create an element
```html
 <div id="bar"></div>
```
Create a new L.Control.Bar object and append to the map  
```javascript
var controlBar = L.control.bar('bar',{
    position:'top',
    visible:true
});
map.addControl(controlBar);
```

### Options
* **position**:
    * top  *(default)*
    * bottom
    * left
    * right

* **visibility**: 
    * true *visible on add (default)*
    * false
 
### Methods
 
~~~~javascript
// Show control bar
controlBar.show();

// Hide control bar
controlBar.hide();

// Toggle control bar visibility
controlBar.toggle();

// Check control bar visibility
var visible = controlBar.isVisible();

// Set content to control bar
controlBar.setContent('<p>This is sample content :)</p>');
~~~~
 
 
### Events

~~~~javascript
controlBar.on('shown', function () {
    console.log('Hello control bar!');
});
~~~~ 

Available events:

- **show**: Show animation is starting, bar will be visible.
- **shown**: Show animation finished, bar is now visible.
- **hide**: Hide animation is starting, bar will be hidden.
- **hidden**: Hide animation finished, bar is now hidden.

 
### License

**leaflet-control-bar** is free software, and may be redistributed under the MIT-LICENSE.

Inspired by [leaflet-sidebar](https://github.com/Turbo87/leaflet-sidebar) plugin.