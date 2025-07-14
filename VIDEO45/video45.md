# CSS Transitions
## Properties
	- Can change way in which an element can act.
	- Having different properties, time-related commands etc.
	- User can vary the changes either in 2D or 3D.

## Example Code
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Transitions</title>
    <style>
        .container{
            background-color: aqua;
            height: 40vh;
            width: 50vw;
        }

        .box{
            background-color: blue;
            height: 4vh;
            width: 5vw;
            /* transition-property: transform;
            transition-duration: 2s;
            transition-timing-function: ease-in-out;
            transition-delay: 1s; */
            transition: all 2s ease-out 1s;
        }

        .translate {
            transform: translateX(10vw) translateY(10vh) scale(2);
            background-color: cadetblue;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="box translate"></div>
    </div>
</body>
</html>
```
