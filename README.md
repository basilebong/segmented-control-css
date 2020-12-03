Create IOS Style radio buttons (segmented controls) without any JavaScript code.

[Official demo](https://codepen.io/basilebong/pen/WBrOjY)

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Installation](#installation)
- [Usage](#usage)
  - [Example](#example)
  - [Colors](#colors)
  - [Animations](#animations)
  - [Border radius](#border-radius)
- [Support](#support)
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

## Usage

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

### Colors

To change the color of the segmented controls add the class `.sc-[colorClass]`.

```html
<div class="segmented-control sc-red">
  <div class="segmented-control-btn">
    <input type="radio" id="react" name="frameworkJs" value="react" checked />
    <label for="react">React</label>
  </div>
</div>
```

|Color name | HEX code | Class |
|-----------|----------| ----- |
| default | #7768ff | sc-default |
| red | #f44335 | sc-red |
| pink | #e81e61 | sc-pink |
| purple | #9b26af | sc-purple |
| deep purple | #663ab6 | sc-deep-purple |
| indigo | #3e50b4 | sc-indigo |
| blue | #2095f2 | sc-blue |
| light blue | #04a8f3 | sc-light-blue |
| cyan | #00bbd3 | sc-cyan |
| teal | #009587 | sc-teal |
| green | #4bad4f | sc-green |
| light green | #8ac249 | sc-light-green |
| lime | #ccdb38 | sc-lime |
| yellow | #feea39 | sc-yellow |
| amber | #fec007 | sc-amber |
| orange | #fe9700 | sc-orange |
| deep orange | #fe5623 | sc-deep-orange |
| brown | #785447 | sc-brown |
| grey | #9d9d9d |  sc-grey |
| blue grey | #5f7c89 | sc-blue-grey |


### Animations

To change the animation of the segmented controls use the class `.sc-[animationClass]`. 

```html
<div class="segmented-control sc-zoom">
  <div class="segmented-control-btn">
    <input type="radio" id="react" name="frameworkJs" value="react" checked />
    <label for="react">React</label>
  </div>
</div>
```

| Name | class |
| ---- | ----------- |
| Fade | sc-fade |
| Slide | sc-slide |
| Zoom | sc-zoom |


### Border radius

| Name | class |
| ---- | ----- |
| Rounded | sc-rounded |
| Round | sc-round |

## Support

Please open an issue for support.

## Author

[Basile Bong](https://basilebong.com)

## License

[MIT](https://en.wikipedia.org/wiki/MIT_License)
