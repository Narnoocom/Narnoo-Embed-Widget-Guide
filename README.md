# Narnoo Widget Guide

The following is a guide on how to use Narnoo's embeddable widgets. This guide has the detailed informatio on these widgets.

## Getting Started

This widget requires a Narnoo account and also at least one developer API key created.


### Narnoo Widget CDN URL

https://booking-widget.narnoo.com/narnoo-widget.min.js

### Narnoo Booking Button Widget CDN URL

https://booking-widget.narnoo.com/booking-button-widget.min.js

### Narnoo Cart Button Widget CDN URL

https://booking-widget.narnoo.com/button-widget.min.js

<br>

# Narnoo Widget Guide

> Example:

``` javascript
<script>
  function(w, d, s, o, f, js, fjs) {
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
      booking_id: "<BOOKING ID>",
      datepicker: true,
      // gallery: false,
      // pricing: false,
      variant: "purple",
      // maxWidth: "200px"
      buttonOptions: {
        label: "Test Booking Label",
        variant: "green",
        // size: "large",
        // fill: "", // clear, outline
        // expand: "block"  
      }
  });
</script>
```
#### [View Guide and Usage Here](https://github.com/Narnoocom/Narnoo-Embed-Widget-Guide/blob/master/widgets/README.md)

<br>

# Narnoo Booking Button Widget Guide

> Example

```javascript
<script>
    function (w, d, s, o, f, js, fjs) {
        w['narnarnoo-booking-button-widget'] = o;
        w[o] = w[o] || function () {
            (w[o].q = w[o].q || []).push(arguments)
        };
        js = d.createElement(s), fjs = d.getElementsByTagName(s)[0];
        js.id = o;
        js.src = f;
        js.async = 1;
        fjs.parentNode.insertBefore(js, fjs);
    }(window, document, 'script', 'narnooBooking', 'https://booking-widget.narnoo.com/booking-button-widget.min.js'));
    narnoo('init', {
        element: "narnoo-button-booking-widget",
        access_key: "<ACCESS_KEY_HERE>",
        operator_id: "<OPERATOR_ID>",
        booking_id: "<BOOKING ID>",
        // label: "Check Availability",
        // variant: "", // green, blue, orange, navy, yellow, peach, red, beige, cyan, celadon, brown, cherry, purple, olive
        // size: "default", // default, small, large
        // expand: "", // block, full
        // fill: "", // clear, outline
        // cssClass: "" // custom CSS Class
    });
</script>
```

#### [View Guide and Usage Here](https://github.com/Narnoocom/Narnoo-Embed-Widget-Guide/blob/master/widget-booking-buttons/README.md)

<br>

# Narnoo Cart Button Widget Guide

> Example

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
#### [View Guide and Usage Here](https://github.com/Narnoocom/Narnoo-Embed-Widget-Guide/blob/master/widget-cart-buttons/README.md)

