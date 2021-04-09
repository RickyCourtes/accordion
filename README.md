# Accordion

Lightweight, fully accessible accordions!

## Install

### Download

+ CSS:
  - [accordion.min.css](https://unpkg.com/@rickycourtes/accordion/dist/accordion.min.css) minified, or
  - [accordion.css](https://unpkg.com/@rickycourtes/accordion/dist/accordion.css) un-minified
  
+ JavaScript:
  - [accordion.min.js](https://unpkg.com/@rickycourtes/accordion/dist/accordion.min.js) minified, or
  - [accordion.js](https://unpkg.com/@rickycourtes/accordion/dist/accordion.js) un-minified

### CDN

Link directly to the Accordion files on unpkg.

``` html 
<!-- CSS -->
<link rel="stylesheet" href="https://unpkg.com/@rickycourtes/accordion/dist/accordion.min.css">
```
``` html
<!-- JavaScript -->
<script src="https://unpkg.com/@rickycourtes/accordion/dist/accordion.min.js"></script>
```

### Package Managers

Install with npm: `npm install @rickycourtes/accordion`

## Usage

Accordion works with a container element and a set of child cell elements

``` html
<div class="accordion">
  <div class="accordion_item">
    <button class="accordion_header">
      <div class="accordion_header__label">Accordion Label</div>
    </button>
    <div class="accordion_panel">
      <div class="accordion_panel_wrap">
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam bibendum rhoncus porta.</p>
      </div>
    </div>
  </div>
  <div class="accordion_item">
    <button class="accordion_header">
      <div class="accordion_header__label">Accordion Label</div>
    </button>
    <div class="accordion_panel">
      <div class="accordion_panel_wrap">
        <p>Aliquam ut neque congue, dapibus sed, lacinia neque. Aliquam eleifend congue malesuada eget.</p>
      </div>
    </div>
  </div>
</div>
```

### Options

#### Initiate with Vanilla JavaScript

You can use Simple Accordion with Vanilla JS by calling `new Accordion()`. The `Accordion()` constructor accepts an options object where you can specify the selector and other options.

``` js
var accordion = new Accordion({
  selector: '.accordion', // Selector can be a string for an idividual element
  singleExpand: false, // Allows only one panel to be exapnded at a time
  expandOnFocus: false, // Expands panels on keyboard focus
});

// OR

var elem = document.querySelector('.accordion');
var accordion = new Accordion({
  selector: elem, // Allows individual element to be passed instead of a string
  singleExpand: false, // Allows only one panel to be exapnded at a time
  expandOnFocus: false, // Expands panels on keyboard focus
});

```
#### Initiate with jQuery

You can use Simple Accordion as a jQuery plugin: $('selector').simpleAccordion().

``` js
$('.accordion').accordion({
  singleExpand: true
});
```

---

By [Ricky Courtes](https://rickycourtes.com)
