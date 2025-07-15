# CSS Animations
## Properties
```
- Different from transitions
- Has more complex properties
- Can be used for different purposes
- Keyframes are used to define an animation
```
## Example Code
```

<style>
      .container {
        background-color: rgb(36, 138, 138);
        height: 80vh;
        width: 30vw;
      }
      .box {
        width: 34px;
        height: 45px;
        /* background-color: beige; */
        animation-name: kuchbhi;
        /* animation-duration: 3s;
            animation-iteration-count: infinite;
            animation-timing-function: cubic-bezier(0, 0.28, 0.46, 0.97);
            animation-delay: 1s;
            animation-direction: reverse;
            animation-play-state: paused; */
        /* animation: name duration timing-function delay iteration-count direction fill-mode; */
        animation: kuchbhi 3s cubic-bezier(0, 0.28, 0.46, 0.97) 1s infinite alternate-reverse, 
                    bakwaas 5s 2;
      }
      @keyframes kuchbhi {
        from {
          /* transform: translateX(1000px); */
          background-color: red;
        }
        to{
            background-color: greenyellow;
            transform: translateX(1000px);
        }
      }
      @keyframes bakwaas{
        0%{
            transform: rotate(50deg);
        }
        20%{
            transform: rotate(90deg);
        }
        50%{
            transform: rotate(120deg);
        }
        70%{
            transform: rotate(180deg);
        }
        100%{
            transform: rotate(270deg);
        }
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="box">Box</div>
    </div>
```
