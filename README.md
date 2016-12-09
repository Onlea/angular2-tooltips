# Angular2 Tooltips

Adapted from bharataj88's [angular2-tooltip](https://github.com/bharatraj88/angular2-tooltip) repo.  Allows for custom placement in parents and manually enable / disable.

## Usage

Add the tooltip attribute with content to an element to display a tooltip on hover.

```html
  <p>
     One word in this sentence will have a
     <span tooltip content="hello">tooltip</span>.
  </p>
```

### Manually Activating
If you don't want to display the tooltip on hover, you can control when it is displayed using the `active` attribute.  The expression passed to the active attribute should be a boolean value.  If it is undefined, the default behaviour for the tooltip will occur (show on hover).

```html
  <p>
     One word in this sentence will have a
     <span tooltip [active]="expression" content="hello">tooltip</span>.
  </p>
```

### Tooltip Class
To change the styling you can add a custom class to the tooltip by passing a class name with the `tooltipClass` attribute.

```html
  <p>
     One word in this sentence will have a
     <span tooltip tooltipClass="custom-tooltip" content="hello">tooltip</span>.
  </p>
```

### DOM Placement
By default the tooltip is appended to the body element.  To append it to a different element, pass a selector using the `parentSelector` attribute.

```html
  <p>
     Only one word in this sentence will have a
     <span tooltip parentSelector="expression" content="hello">tooltip</span>.
  </p>
```
