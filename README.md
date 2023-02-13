# Hover.scss

This is a fork of [Ian Lunn's Hover](https://github.com/IanLunn/Hover) customised for use in my SASS-based projects, such as WordPress themes using my [starter kit](https://github.com/doubleedesign/doublee-dev-starter-kit).

For use in your own projects please ensure you have an appropriate [license from Ian](https://ianlunn.co.uk/store/licenses/).


## Setup
```json5
// In package.json
"dependencies": {
    "@doubleedesign/hover.css": "https://github.com/doubleedesign/Hover.css#1.0.0"
},
```
```scss
@import '../node_modules/@doubleedesign/hover.scss/hover'; // alter path to node_modules as per your project structure
```
This project assumes that [Font Awesome 6](https://www.fontawesome.com) is present in the project if using  the icon effects.

## Usage

The main way this fork differs from the original Hover.css is the availability of an optional colour parameter when you call the mixin.
```scss
.btn {
    @include sweep-to-right($primary-color);
}
```

If you don't set this, it will default to `$activeColor` as per the original Hover.css.

You can also change Font Awesome icon weight by setting the variable `$fa-default-weight`.
