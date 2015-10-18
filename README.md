# Pinch Zoom Background Image - jQuery plugin


## Installation

Clone this [repository](https://github.com/nadeeth/pinch-zoom.git) or download the [latest build](https://github.com/nadeeth/pinch-zoom/archive/master.zip).

Include jQuery library and google maps API places library:

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.2/jquery.min.js"></script>
```

Include pinch-zoom.js *after* the jQuery library:

```html
<script src="/path/to/pinch-zoom.js"></script>
```

## Usage

```javascript
$(function() {
    $("#wrap").pinchzoom(); // 'wrap' is the id of the div with the background image to be pinched. 
});
```

## Options

### width

    width : 500

When this option is provided, width of background will be reseted before starting zoom.

Ex: 
```javascript
$("#wrap").pinchzoom({
    width : 500
});
```

### done

    done : function

A callback function to run after the zooming is done.

Ex: 
```javascript
$("#wrap").pinchzoom({
    done : function() {
        var size = $("#wrap").css("background-size");
        //Do Something
});
```

### min_width

    min_width : 200

Minimum size to zoom in. Image will not shrink below this size. Default is 50 pixels. 

Ex: 
```javascript
$("#wrap").pinchzoom({
    min_width : 200
});
```
