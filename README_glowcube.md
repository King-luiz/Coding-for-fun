# Glowing Cube Project

This project showcases a **glowing, rotating 3D cube** created entirely with HTML and CSS. It demonstrates advanced CSS techniques such as animations, 3D transformations, and the use of custom properties (CSS variables). The project is designed to help users understand and explore the power of CSS styling and animation.

## Features

- **3D Transformations**: The cube rotates on the X and Y axes, giving it a dynamic and realistic 3D appearance.
- **CSS Animations**: Smooth, infinite rotation of the cube using `@keyframes` and `animation` properties.
- **Glowing Effect**: The top face of the cube emits a glowing effect with multiple layers of `box-shadow` and `filter: blur()`.
- **CSS Variables**: Custom properties (`--bg-color`) are used to simplify and centralize color management.
- **Modern Design**: Clean and minimalistic design with radial gradient backgrounds for enhanced visual appeal.

## Code Breakdown

### HTML Structure

The HTML defines a `div` element for the cube and its faces:

```html
<div class="cube">
    <div class="top"></div>
    <div>
        <span style="--i:0"></span>
        <span style="--i:1"></span>
        <span style="--i:2"></span>
        <span style="--i:3"></span>
    </div>
</div>
```

### CSS Styling

#### Background
A radial gradient creates a visually appealing background:

```css
body {
    --bg-color: radial-gradient(rgb(15, 14, 14), #0b0a0a);
    background: var(--bg-color);
}
```

#### Cube Rotation
The `@keyframes` animation rotates the cube infinitely on the Y-axis:

```css
@keyframes animate {
    0% {
        transform: rotateX(-30deg) rotateY(-1000deg);
    }
    100% {
        transform: rotateX(-30deg) rotateY(-380deg);
    }
}
```

#### Glowing Effect
The glowing effect on the top face is achieved using `box-shadow` and `filter`:

```css
.top::before {
    box-shadow: 0 0 120px rgba(0, 255, 0, 0.2),
                0 0 200px rgba(0, 255, 0, 0.4),
                0 0 300px rgba(0, 255, 0, 0.6),
                0 0 400px rgba(0, 255, 0, 0.8),
                0 0 500px rgba(0, 255, 0, 1);
}
```

## Purpose

This project demonstrates my CSS skills, including:

- Mastery of animations and 3D transformations.
- Advanced use of shadows, gradients, and filters to create glowing effects.
- Understanding of CSS variables for clean and maintainable code.

## How to Use

1. Copy the provided HTML and CSS code into a `.html` file.
2. Open the file in a modern web browser (e.g., Chrome, Firefox).
3. Enjoy the glowing, rotating cube!

## Future Improvements

- Add user interaction (e.g., rotate the cube with mouse or touch gestures).
- Include additional glowing elements or dynamic colors.
- Provide more customization options using CSS variables.

## Acknowledgments

This project is part of my journey to showcase and improve my front-end development skills. Feel free to share feedback or suggestions!

##Demo

You can view the project in action by opening the HTML file in any modern web browser.

Video Preview



https://github.com/user-attachments/assets/d7ab204c-98ca-4190-a2fd-2a93ad3e6e08



Download or clone the repository to run the code locally.




