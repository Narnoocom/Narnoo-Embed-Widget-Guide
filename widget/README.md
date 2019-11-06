# Narnoo Widget

Our most detailed widget. This embed widget displays a booking form on the page which shows a number of different booking display options.

## Narnoo Widget CDN URL

https://booking-widget.narnoo.com/narnoo-widget.min.js

#### Add this element on inside the html `body`

```html
<div id="narnoo-js-widget"></div>
```
<b>Note:</b> You can replace any ID value for the div element

### Usage

```javascript
<script>
    function (w, d, s, o, f, js, fjs) {
        w['narnoo-widget'] = o;
        w[o] = w[o] || function () {
            (w[o].q = w[o].q || []).push(arguments)
        };
        js = d.createElement(s), fjs = d.getElementsByTagName(s)[0];
        js.id = o;
        js.src = f;
        js.async = 1;
        fjs.parentNode.insertBefore(js, fjs);
    }(window, document, 'script', 'narnoo', 'https://booking-widget.narnoo.com/narnoo-widget.min.js'));
    narnoo('init', {
        element: "narnoo-js-widget",
        access_key: "<ACCESS_KEY_HERE>",
        operator_id: "<OPERATOR_ID>",
        product_id: "<BOOKING ID>",
        datepicker: true,
        pricing: false,
        //gallery: false,
        // maxWidth: "400px",
        // variant: "",
        // optionButtons: {}
    });
</script>
```

### Widget Configuration

#### init Properties

| **Option**  |  **Details**|
|------------|---|
|   `element` | `**required**` <small>This the element ID where the widget will be rendered.</small> |
| `access_key` | <small>This is the widget `access_key` to authorize for API request</small>  |
| `operator_id` | <small>This is the widget `operator_id` to authorize for API request</small>  |
| `product_id` | <small>This is the widget `product_id` to authorize for API request</small>  |
| `datepicker` | <small>If `true`, widget will display a datepicker as part on filtering. </small>  |
| `gallery` | <small>If `true`, widget will display a carousel of images or a featured image for additional display of information. </small>  |
| `pricing` | <small>If `true`, widget will display a list of selected product option prices </small>  |
| `maxWidth` | <small>Sets a maximum width on the Widget.</small>  |
| `variant`  | <small> Default options are: `main`, `green`, `blue`, `orange`, `navy` ,`yellow`, `peach`, `red`, `beige`, `cyan`, `celadon`, `brown`, `cherry`, `purple`, `olive`</small> |
| `optionButtons` | <small>This the widget button option properties to configure its theme, design and position. See Option properties below.</small>  |



### Properties

**element**

|   | |
|------------|---|
|  Description | <small>This the element ID where the widget will be rendered</small> |
| Attribute | `element`  |
| Usage | <small>See below example. </small>  |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
});
```

**access_key**

|   | |
|------------|---|
|  Description | <small>This is the widget `access_key` to authorize for API request</small> |
| Attribute | `access_key`  |
| Type | `string` or `undefined`  |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>"
});
```

**operator_id**

|   | |
|------------|---|
|  Description | <small>This is the widget `operator_id` to authorize for API request</small> |
| Attribute | `operator_id`  |
| Type | `string` or `undefined`  |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
});
```

**product_id**

|   | |
|------------|---|
|  Description | <small>This is the widget `product_id` to authorize for API request</small> |
| Attribute | `product_id`  |
| Type | `string` or `undefined`  |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
    product_id: "<BOOKING ID>"
});
```


**datepicker**

|   | |
|------------|---|
|  Description | <small>If `true`, widget will display a datepicker as part on filtering. </small> |
| Attribute | `datepicker`  |
| Type | `boolean`  |
| Default | `true` |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
    product_id: "<BOOKING ID>",
    datepicker: true
});
```

**gallery**

|   | |
|------------|---|
|  Description | <small>If `true`, widget will display a carousel of images or a featured image for additional display of information. </small> |
| Attribute | `gallery`  |
| Type | `boolean`  |
| Default | `true` |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
    product_id: "<BOOKING ID>",
    datepicker: true,
    gallery: false
});
```

**pricing**

|   | |
|------------|---|
|  Description | <small>If `true`, widget will display a list of prices base on selected product option </small> |
| Attribute | `pricing`  |
| Type | `boolean`  |
| Default | `false` |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
    product_id: "<BOOKING ID>",
    datepicker: true,
    gallery: false,
    pricing: true
});
```

**maxWidth**

|   | |
|------------|---|
|  Description | <small>Sets a maximum width of the widget</small> |
| Attribute | `maxWidth`  |
| Type | `string` or `undefined`  |
| Default | `400px`  |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
    product_id: "<BOOKING ID>",
    datepicker: true,
    gallery: false,
    maxWidth: "400px"
});
```

**variant**

|   | |
|------------|---|
|  Description | <small>The color to use from your widget. Default options are: `main`, `green`, `blue`, `orange`, `navy` ,`yellow`, `peach`, `red`, `beige`, `cyan`, `celadon`, `brown`, `cherry`, `purple`, `olive`</small> |
| Attribute | `variant`  |
| Values | `main` , `green` , `blue` , `orange` , `navy` , `yellow` , `peach` , `red` , `beige` , `cyan` , `celadon` , `brown` , `cherry` , `purple` , `olive` |
| Type | `string` or `undefined`  |
| Default | `main`  |


``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
    product_id: "<BOOKING ID>",
    datepicker: true,
    gallery: false,
    maxWidth: "400px",
    variant: "main"
});
```

**optionButtons**

|   | |
|------------|---|
|  Description | <small>This the widget button option properties to configure its theme, design and position. See optionButtons properties below.</small> |
| Attribute | `optionSize`  |
| Type | `object` or `undefined`  |
| Values | See option properties below.  |

``` javascript
narnoo('init', {
    element: "narnoo-js-widget",
    access_key: "<ACCESS_KEY_HERE>",
    operator_id: "<OPERATOR_ID>",
    product_id: "<BOOKING ID>",
    datepicker: true,
    gallery: false,
    maxWidth: "400px",
    variant: "main",
    optionButtons: {
      label: "Check Availability",
      variant: "", // Button variant can be inherited on the widget variant. Can be set also its own variant
      size: "default", // default, small, large
      expand: "", // block, full
      cssClass: "", // custom CSS Class
    }
});
```

#### optionButtons Properties

| **Value**  |  **Details**|
|------------|---|
|   `label` | <small>Button label or caption</small> |
| `variant`  | <small> Default options are: `main`, `green` ,`blue` ,`orange` ,`navy` ,`yellow` ,`peach` ,`red` ,`beige` ,`cyan` ,`celadon` ,`brown` ,`cherry` ,`purple` ,`olive`</small> |
| `size` | <small>This attribute specifies the size of the button. Setting this attribute will change the height and padding of a button.</small>  |
| `expand` | <small>This attribute lets you specify how wide the button should be. By default, buttons are inline blocks, but setting this attribute will change the button to a full-width block element.</small>  |
| `cssClass` | <small>Additional classes to apply for custom CSS. If multiple classes are provided they should be separated by spaces.</small>  |

<br>

##### `size` optionButton Properties

| **Value**  |  **Details**|
|------------|---|
|   `small` | <small>Button with less height and padding. Default for buttons in an item.</small> |
| `default`  | <small>Button with the default height and padding. Useful for buttons in an item.</small> |
| `large` | <small>Button with more height and padding.</small>  |


##### `expand` optionButton Properties

| **Value**  |  **Details**|
|------------|---|
|   `block` | <small>Full-width button with rounded corners.</small> |
| `full`  | <small>Full-width button with square corners and no border on the left or right.</small> |
