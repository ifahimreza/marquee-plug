# MarqueePlug

MarqueePlug is an easy-to-use, customizable, and lightweight JavaScript library for creating marquee effects.

## Features

-   Auto-fill: Automatically fills the blank space in the marquee with copies of the children.
-   Play/Pause: Play or pause the marquee animation.
-   Pause on Hover/Click: Pause the marquee when hovered or clicked.
-   Direction: Control the direction of the marquee.
-   Speed: Set the speed of the marquee animation.
-   Gradient: Add gradient overlay for a smooth visual effect.
-   Callback Functions: Add callbacks for loop completion and finishing.

## Usage

To use MarqueePlug in your project, follow these steps:

### NPM

The recommended installation method is NPM. Install the latest version with the following command:

```bash
$ npm install marquee-plug
```

### Hosting Files

You can download the MarqueePlug package from the following link:

Download

Go to the dist directory, and import the marquee-plug.min.js file with the <script> tag:

```js
<script src="path-to-the-file/marquee-plug.min.js"></script>
```

### Basic Example

Here's a basic example of how to use MarqueePlug:

HTML: Add a container for the marquee effect.

```html
<div id="marquee-container" class="marquee">
	<p>Your scrolling text goes here.</p>
	<p>Your scrolling text goes here.</p>
</div>
```

JavaScript: Initialize MarqueePlug on your elements.

```js
const marquee = new MarqueePlug('#marquee-container', {
	autoFill: true, // Automatically fills the marquee with content
	speed: 50, // Speed of the marquee
	direction: 'left', // Direction of the marquee (left, right, up, down)
});

marquee.init();
```

## Files

You will find two files in the dist directory:

-   marquee-plug.min.js
-   marquee-plug.css

## Options

### `autoFill` (boolean)

**Description**: Automatically fills blank space in the marquee with copies of the children.
**Default**: `false`
**Example**: `autoFill: true`

### `play` (boolean)

**Description**: Whether to play or pause the marquee.
**Default**: `true`
**Example**: `play: false`

### `pauseOnHover` (boolean)

**Description**: Whether to pause the marquee when hovered.
**Default**: `false`
**Example**: `pauseOnHover: true`

### `pauseOnClick` (boolean)

**Description**: Whether to pause the marquee when clicked.
**Default**: `false`
**Example**: `pauseOnClick: true`

### `direction` (string)

**Description**: The direction the marquee is sliding.
**Options**: `"left"`, `"right"`, `"up"`, `"down"`
**Default**: `"left"`
**Example**: `direction: 'right'`

### `speed` (number)

**Description**: Speed calculated as pixels/second.
**Default**: `50`
**Example**: `speed: 100`

### `delay` (number)

**Description**: Duration to delay the animation after render, in seconds.
**Default**: `0`
**Example**: `delay: 2`

### `loop` (number)

**Description**: The number of times the marquee should loop. `0` is equivalent to infinite.
**Default**: `0`
**Example**: `loop: 3`

### `gradient` (boolean)

**Description**: Whether to show the gradient or not.
**Default**: `false`
**Example**: `gradient: true`

### `gradientColor` (string)

**Description**: The color of the gradient.
**Default**: `"white"`
**Example**: `gradientColor: 'rgba(255, 255, 255, 0.5)'`

### `gradientWidth` (number|string)

**Description**: The width of the gradient on either side.
**Default**: `200`
**Example**: `gradientWidth: '10%'`
