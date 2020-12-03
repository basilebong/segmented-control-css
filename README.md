![Segmented Control CSS](thumb.jpg)

Create IOS Style radio buttons (segmented controls) without any JavaScript code.

[Official demo](https://codepen.io/basilebong/pen/WBrOjY)

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Installation](#installation)
- [Getting started](#getting-started)
  - [Example](#example)
- [Support](#support)
- [Contributing](#contributing)
- [Author](#author)
- [License](#license)

## Installation

```shell
npm i segmented-control-css
```

```shell
yarn add segmented-control-css
```

Then add the `segmented-control.min.css` file to your `<head>`. The file is located in the `dist` folder.

```html
<link
  rel="stylesheet"
  href="[path-to-segmented-control-css]/dist/segmented-control.min.css"
/>
```

You can also use the `unpkg` CDN.

```html
<link
  rel="stylesheet"
  href="https://unpkg.com/segmented-control-css/dist/segmented-control.min.css"
/>
```

## Getting started

To make Segmented Control CSS work properly:

- All options are grouped inside an `.segmented-control` container.
- Each option should have:
  - A `.segmented-control-btn` wrapper.
  - An `<input type="radio">` with an **unique id**.
  - A `<label>` with a for attribute

⚠️ Each `.segmented-control-btn` needs an **input with an id** and a label **just behind**. The "for" attribute of the label needs to be **the same as the id** of the input. ⚠️

### Example

```html
<form>
  <div class="segmented-control">
    <div class="segmented-control-btn">
      <input type="radio" id="react" name="frameworkJs" value="react" checked />
      <label for="react">React</label>
    </div>
    <div class="segmented-control-btn">
      <input type="radio" id="angular" name="frameworkJs" value="angular" />
      <label for="angular">Angular</label>
    </div>
    <div class="segmented-control-btn">
      <input type="radio" id="vue" name="frameworkJs" value="vue" />
      <label for="vue">Vue</label>
    </div>
  </div>
</form>
```

## Support

Please open an issue for support.

## Contributing

Please contribute using [Github Flow](https://guides.github.com/introduction/flow/). Create a feature/branch, add commits, and open a pull request.

## Author

[Basile Bong](https://basilebong.com)

## License

[MIT](https://en.wikipedia.org/wiki/MIT_License)
