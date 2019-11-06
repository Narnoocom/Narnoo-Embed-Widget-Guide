# Narnoo Cart Button Widget

The Narnoo cart button outputs a button on the page which allows the user to open up their cart containing their selected products.


## Narnoo Cart Button Widget CDN URL

https://booking-widget.narnoo.com/button-widget.min.js


#### Add this element on inside the html `body`

```html
<div id="narnoo-button-booking-widget"></div>
```

<b>Note:</b> You can replace any ID value for the div element

### Usage

```javascript
<script>
    function (w, d, s, o, f, js, fjs) {
        w['narnoo-button-widget'] = o;
        w[o] = w[o] || function () {
            (w[o].q = w[o].q || []).push(arguments)
        };
        js = d.createElement(s), fjs = d.getElementsByTagName(s)[0];
        js.id = o;
        js.src = f;
        js.async = 1;
        fjs.parentNode.insertBefore(js, fjs);
    }(window, document, 'script', 'narnooButton', 'https://booking-widget.narnoo.com/button-widget.min.js'));
    narnoo('init', {
        element: "narnoo-button-cart-widget",
        label: "View Cart with label",
        size: "small", // small, default, large
        // variant: "", // green, blue, orange, navy, yellow, peach, red, beige, cyan, celadon, brown, cherry, purple, olive
        // size: "default", // default, small, large
        // expand: "", // block, full
        // fill: "", // clear, outline
        // cssClass: "" // custom CSS Class
    });
</script>
```

### Widget Configuration

#### init Properties

| **Option**  |  **Details**|
|------------|---|
|   `element` | `**required**` <small>This the element ID where the widget will be rendered.</small> |
|   `label` | <small>Button label or caption</small> |
| `variant`  | <small> Default options are: `main`, `green` ,`blue` ,`orange` ,`navy` ,`yellow` ,`peach` ,`red` ,`beige` ,`cyan` ,`celadon` ,`brown` ,`cherry` ,`purple` ,`olive`</small> |
| `size` | <small>This attribute specifies the size of the button. Setting this attribute will change the height and padding of a button.</small>  |
| `expand` | <small>This attribute lets you specify how wide the button should be. By default, buttons are inline blocks, but setting this attribute will change the button to a full-width block element.</small>  |
| `fill` | <small>This attributes determines the background and border color of the button. By default, buttons have a solid background unless the button is inside of a toolbar, in which case it has a transparent background. Options are `clear`, `outline`, `default`</small>  |
| `cssClass` | <small>Additional classes to apply for custom CSS. If multiple classes are provided they should be separated by spaces.</small>  |

### Properties

**element**

|   | |
|------------|---|
|  Description | <small>This the element ID where the widget will be rendered</small> |
| Attribute | `element`  |
| Usage | <small>See below example. </small>  |

``` javascript
narnoo('init', {
    element: "narnoo-button-cart-widget",
});
```

**label**

|   | |
|------------|---|
|  Description | <small>Button Label or Caption</small> |
| Attribute | `label`  |
| Type | `string` or `undefined`  |
| Default | `Check Availability`  |

``` javascript
narnoo('init', {
    element: "narnoo-button-cart-widget",
    label: "Check Availability"
});
```

**size**

| **Option**  |  **Details**|
|------------|---|
| Attribute | `size`  |
| Type | `string` or `undefined`  |
| Default | `default`  |
|||
| **Value**  |  **Details**|
|||
|   `small` | <small>Button with less height and padding. Default for buttons in an item.</small> |
| `default`  | <small>Button with the default height and padding. Useful for buttons in an item.</small> |
| `large` | <small>Button with more height and padding.</small>  |

``` javascript
narnoo('init', {
    element: "narnoo-button-cart-widget",
    label: "Check Availability"
    size: "default" // If no value, then it will use the `default` button size
});
```

**expand**

| **Option**  |  **Details**|
|------------|---|
| Attribute | `expand`  |
| Type | `string` or `undefined`  |
|||
| **Value**  |  **Details**|
|||
|   `block` | <small>Full-width button with rounded corners.</small> |
| `full`  | <small>Full-width button with square corners and no border on the left or right.</small> |

``` javascript
narnoo('init', {
    element: "narnoo-button-cart-widget",
    label: "Check Availability"
    size: "default", // If no value, then it will use the `default` button size
    expand: "block" // If no value, then it will use the default button wide aspect
});
```

**fill**

| **Option**  |  **Details**|
|------------|---|
|  Description | <small>Set to `clear` for a transparent button, to `outline` for a transparent button with a border, or to `default`. The default style is `default`</small> |
| Attribute | `fill`  |
| Type | `clear` or `outline` or `default` or `undefined` |
|||
| **Value**  |  **Details**|
|||
|   `clear` | <small>Button with a transparent background that resembles a flat button.</small> |
| `outline`  | <small>Button with a transparent background and a visible border.</small> |
| `default`  | <small>Button with a filled background.</small> |

``` javascript
narnoo('init', {
    element: "narnoo-button-booking-widget",
    access_key: "<ACCESS_KEY_HERE>",
    label: "Check Availability"
    size: "default", // If no value, then it will use the `default` button size
    expand: "block", // If no value, then it will use the default button wide aspect
    fill: "default"
});
```

**cssClass**

|   | |
|------------|---|
|  Description | <small>Additional classes to apply for custom CSS. If multiple classes are provided they should be separated by spaces.</small> |
| Attribute | `cssClass`  |
| Type | `string` or `string[]` or `undefined`  |

``` javascript
narnoo('init', {
    element: "narnoo-button-cart-widget",
    label: "Check Availability",
    size: "default", // If no value, then it will use the `default` button size
    expand: "block" // If no value, then it will use the default button wide aspect
    cssClass: "custom-class-here",
    fill: "default"
});
```
