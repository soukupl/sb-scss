# SCSS mixin library

This is set of SCSS mixins, that you can simply use in your own SCSS code.
> NOTE: This is work in progress, not all mixins are documented and may not work. At this point, use at your won risk!

## Install

1. `npm install sb-scss --save-dev`
2. In your SCSS file, just import `@import "sb-scss";`

---

## Contrast color

`choose-contrast-color($color)`

This function will calculate contrast color to passed color. Useful to automaticaly switch text color from black to white depending on the background color.

This will always return 'black' or 'white'.

```scss
.should-be-white {
  color: choose-contrast-color(#111111);
}
```

<p align="center">⬇️</p>

```css
.should-be-white {
  color: white;
}
```

## Animations

Typewritter FX

```scss
.title {
  @include typewriter(#f00, 300px, 50);
}
```
