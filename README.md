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

### Importing MarqueePlug

You can install MarqueePlug using npm:

    ```bash
    npm install marquee-plug
    ```

    ```javascript
    import MarqueePlug from 'marquee-plug';
    ```

    ```html
    <script src="marquee-plug.js"></script>
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

Initialize MarqueePlug on your elements.

    ```javascript
    const marquee = new MarqueePlug('#marquee-container', {
    	autoFill: true, // Automatically fills the marquee with content
    	speed: 50, // Speed of the marquee
    	direction: 'left', // Direction of the marquee (left, right, up, down)
    });

    marquee.init();
    ```

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

### `onFinish` (function)

**Description**: A callback for when the marquee finishes scrolling and stops. Only calls if loop is non-zero.
**Default**: `null`
**Example**: `onFinish: () => { console.log('Marquee finished'); }`

### `onCycleComplete` (function)

**Description**: A callback for when the marquee finishes a loop. Does not call if maximum loops are reached (use onFinish instead).
**Default**: `null`
**Example**: `onCycleComplete: () => { console.log('Marquee cycle complete'); }`

```

```
