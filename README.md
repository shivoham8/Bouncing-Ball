# Animated Floating Ball

## HTML Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <div class="ball"></div>
    </div>
</body>
</html>
```

## CSS Code
```css
html {
    overflow: hidden;
}

.container {
    position: relative;
    height: 80vh;
    width: 80vw;
    background-color: rgb(126, 240, 202);
}

.ball {
    height: 121px;
    width: 121px;
    background-color: rgb(221, 95, 95);
    border-radius: 70px;
    position: absolute;
    bottom: 0;
    left: 0;
    animation: y-axis 1s ease-out infinite alternate,
               x-axis 3s linear infinite;            
}

@keyframes y-axis {
    from {
        bottom: 0;
    }  
    to {
        bottom: 100%;
    }
}

@keyframes x-axis {
    from {
        left: 0;
    }
    to {
        left: 100%;
    }
}
```

## Animation Description

- The provided CSS code creates an animated floating ball.
- The ball moves upward along the y-axis and simultaneously from left to right along the x-axis in an infinite loop.
- This animation adds a dynamic and visually appealing element to a webpage.
- Adjustments to colors, sizes, or animation durations can be made for customization.

## How to Use

1. Copy the CSS code into a separate file or section of your HTML file.
2. Apply the styles to the desired HTML element, such as a <div> with the class "ball".
3. Adjust the container size, ball size, colors, or animation durations to fit your design preferences.

## Features

- **Fluid animation:** The box smoothly floats upward and across the screen.
- **Customizable:** Easily adjust container size, box size, colors, or animation durations to fit design preferences.
- **Simple integration:** Copy and paste the provided HTML and CSS code into your project for quick implementation.

Feel free to use and modify this code to enhance the visual appeal of your web projects. Explore different color schemes, sizes, and durations to create a unique animated effect.
