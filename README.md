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

