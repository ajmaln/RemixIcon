<p align="left">
    <a href="https://remixicon.com/"><img src="http://pk6meb1tz.bkt.clouddn.com/github-logo.svg" alt="remixicon" width=280 height=64></a>
    <p align="left">Remix Icon is a set of open source neutral style system symbols for designers and developers. Unlike a patchwork icon library, More than 1200 icons are all elaborately crafted so that they are born with the gene of readability, consistency and perfect pixels. Each icon was designed in "Outlined" and "Filled" styles based on a 24x24 grid. Of course, all the icons are free to use for both personal and commercial.</p>
    <p>View the full set of Remix Icons at <a href="https://remixicon.com">remixicon.com</a>.</p>
</p>

## Usage

### Basic Usage
Just click the icons you want from [remixicon.com](https://remixicon.com), and the icons will be downloaded directly in SVG format.

> We recommend that designers download icons from our website when needed instead of managing all of them in a local folder. The website's search engine allows you to quickly locate the icon you are looking for and the icons in the website are continuously updating.

Preparing an SVG for use on the web is a simple process and no more complicated that exporting a JPEG or PNG. Such as:

```
<img height="32" width="32" src="img/admin-fill.svg" />
```

### Webfont Usage

#### Installation
> **Note:** If you'd like to use Remix Icon with a CDN, you can skip this installation step.

```
npm install remixicon --save
```

```
import 'remixicon/fonts/remixicon.css'
```
> import CSS to your main.js

#### CDN
Copy the following code and add it to the <head> tag of your html document.
```
<link href="https://remixicon.com/fonts/remixicon.css" rel="stylesheet">
```

#### Use
Add icon with class name, class name rule: remixixon-${name}-${style}
```
<i class="remixicon-admin-line"></i>
<i class="remixicon-admin-fill"></i>
```
> **Note:** You can go to [remixicon.com](https://remixicon.com) to check the name of the icons. `-line` means the outlined style icon, and `-fill` means the filled style icon.

### SVG Sprite Usage
Download [`remixicon.symbol.svg`](http://remixicon.com/fonts/remixicon.symbol.svg) file into your project directory，use icons with the `<use>` element, such as:

```css
.remix {
  width: 24px;
  height: 24px;
  fill: #333;
}
```

```html
<svg class='remix'>
  <use xlink:href="remixicon.symbol.svg#remixicon-admin-fill"></use>
</svg>
```

> **Note:** `remixicon-admin-fill` after the '#' in the above example can be replaced with any valid icon name of Remix Icon. You can go to [remixicon.com](https://remixicon.com) to check the name of the icons. `-line` means the outlined style icon, and `-fill` means the filled style icon.
