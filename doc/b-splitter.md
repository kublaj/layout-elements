{
  title: "Splitter",
  element: 'b-splitter',
  category: "elements",
  section: "layout",
  order: 2
}

# b-splitter

`b-splitter` is a split bar that can be used for resizing a sibling element, which is defined by the value of the `direction` attribute. It is to be used with a flexible layout, such as one provided by `b-linear-layout` for instance.

## Usage

``` html
<b-linear-layout>
    <div style="min-width: 100px;">Left (min: 100px)</div>
    <b-splitter direction="left"></b-splitter>
    <div expand>Right</div>
</b-linear-layout>
```

In the above sample, the splitter will resize the left element. Since the right element is set to `expand`, it will be automatically resized when the left one is resized. If you specify a `min-width` for the element to be resized, this minimum width will be enforced by the splitter.

When resizing, some element's contents may overflow outside of the element, so you may need to set this element to `overflow: hidden` or `overflow: scroll` depending on your preferences.

## API

### Attributes
- __direction__: specifies the sibling to resize. Possible values: `left`, `right`, `up`, `down` (default: `left`).


