leaflet-control-bar
=====================

Simple bar for [Leaflet](http://leafletjs.com).

*Requires Leaflet 0.7.0 or newer and modern browser*

## Using the plugin


### Usage

**You have to request your API key! For more info please contact the developer.**

Available position option
 * top  *(default)*
 * bottom
 * left
 * right
 
Create an element
```html
 <div id="bar"> ... </div>
```

Create a new L.Control.Bar object and append to the map  
```javascript
var controlBar = L.control.bar('bar',{
    position:'top',
    visible:true
});
map.addControl(controlBar);
```

### License

**leaflet-control-bar** is free software, and may be redistributed under the MIT-LICENSE.

