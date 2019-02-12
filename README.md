# div placeholder

**Quite practical CSS solution to add placeholder "div" element with empty content. No Javascript required.**

[Codepen Demo](https://codepen.io/rahmanyerli/pen/BMVKZm)

```html
<div data-placeholder="placeholder text..."></div>
```

```css
div {
    margin: 1rem;
    padding: 1rem;
    border: 1px solid #000000;
    font-family: sans-serif;
}

div:empty:not(:focus):before {
    content: attr(data-placeholder);
    color: #999999;
}
```
