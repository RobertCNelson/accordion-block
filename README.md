# Accordion Block

Simple Accordion component plugin for GrapesJS


[Demo](http://grapesjs.com/demo.html)


## Requirements
* GrapesJS v0.13.8 or higher


## Summary

* Plugin name: `grapesjs-accordions`
* Components
  * `accordions` - Main accordions component
  * `accordion-container` - Component which contains a single accordion
  * `accordion` - Single accordion component
  * `accordion-content` - Accordion's content
* Blocks
  * `accordions`





## Options

|Option|Description|Default|
|-|-|-
| `accordionsBlock` | Object to extend the default accordions block, eg. `{ label: 'Accordions', attributes: { ... } }`. Pass a falsy value to avoid adding the block| `{}` |
| `accordionsProps` | Object to extend the default accordions properties, eg. `{ name: 'My Accordions', droppable: false, ... }` | `{}` |
| `accordionProps` | Object to extend the default accordion properties | `{}` |
| `accordionContentProps` | Object to extend the default accordion content properties | `{}` |
| `accordionContainerProps` | Object to extend the default accordion container properties | `{}` |
| `attrAccordions` | Accordions attribute identifier (main component) | `data-accordions` |
| `attrAccordion` | Accordion attribute identifier | `data-accordion` |
| `attrAccordionContent` | Accordion content attribute identifier | `data-accordion-content` |
| `attrAccordionContainer` | Accordion container attribute identifier | `data-accordion-container` |
| `classAccordion` | Default class to use on accordion | `accordion` |
| `classAccordionActive` | Class used on accordions when active | `accordion-active` |
| `classAccordionContent` | Default class to use on accordion content | `accordion-content` |
| `classAccordionContainer` | Default class to use on accordion container | `accordion-container` |
| `selectorAccordion` | The attribute used inside accordions as a selector for accordion contents | `href` |
| `template` | Default accordions template | `<nav ....` (check the source) |
| `templateAccordionContent` | Default template for new added accordion contents | `<div>New Accordion Content</div>` |
| `style` | Default style for accordions | `.accordion { ....` (check the source) |



## Download

* GIT
  * `git clone https://github.com/blairpanek/accordion-block.git`





## Usage

```html
<link href="https://unpkg.com/grapesjs/dist/css/grapes.min.css" rel="stylesheet"/>
<script src="https://unpkg.com/grapesjs"></script>
<script src="path/to/accordion-block.min.js"></script>

<div id="gjs"></div>

<script type="text/javascript">
  var editor = grapesjs.init({
      container : '#gjs',
      ...
      plugins: ['accordion-block'],
      pluginsOpts: {
        'accordion': {
          // options
        }
      }
  });
</script>
```





## Development

Clone the repository

```sh
$ git clone https://github.com/blairpanek/accordion-block.git
$ cd into cloned repository
```

Install dependencies

```sh
$ npm i
```

The plugin relies on GrapesJS via `peerDependencies` so you have to install it manually

```sh
$ npm i grapesjs --no-save
```

Start the dev server

```sh
$ npm start
```





## License

BSD 3-Clause
