# canvas-confetti

## Demo

[catdad.github.io/canvas-confetti](https://catdad.github.io/canvas-confetti/)

## API

This library is exposed as a `confetti` function on `window`. It takes a single optional `options` object, which has the following properties:

- `particleCount` _Integer (default: 50)_: The number of confetti to launch. More is always fun... but be cool, there's a lot of math involved.
- `angle` _Number (default: 90)_: The angle in which to launch the confetti, in degrees. 90 is straight up.
- `spread` _Number (default: 45)_: How far off center the confetti can go, in degrees. 45 means the confetti will launch at the defined `angle` plus or minus 22.5 degrees.
- `startVelocity` _Number (default: 45)_: How fast the confetti will start going, in pixels.
- `decay` _Number (default: 0.9)_: How quickly the confetti will lose speed. Keep this number between 0 and 1, otherwise the confetti will gain speed. Better yet, just never change it.
- `ticks` _Number (default: 200)_: How many times the confetti will move. This is abstract... but play with it if the confetti disappear too quickly for you.
- `origin` _Object_: Where to start firing confetti from. Feel free to launch off-screen if you'd like.
  - `origin.x` _Number (default: 0.5)_: The `x` position on the page, with `0` being the left edge and `1` being the right edge.
  - `origin.y` _Number (default: 0.5)_: The `y` position on the page, with `0` being the top edge and `1` being the bottom edge.
- `colors` _Array&lt;String&gt;_: An array of color strings, in the HEX format... you know, like `#bada55`.
