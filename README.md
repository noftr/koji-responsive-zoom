# koji-responsive-zoom

This library allows for responsive layout without issues related to zoom support in the browser.

## Usage

Add the following code to your page:

```js
let windowWidth = window.outerWidth;
window.addEventListener("resize", () => {
  if (windowWidth !== window.outerWidth) {
    setFontSize();
  }
  windowWidth = window.outerWidth;
});
function setFontSize() {
  const vwSize = window.innerWidth / 100;
  document.documentElement.style.fontSize = vwSize + "px";
  document.body.style.fontSize = vwSize + "px";
}
setFontSize();
```

## License

MIT License
