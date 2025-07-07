# CSS Grid
## Properties
- Divided elements into grid items.
- Can be kept anywhere in the grid.
- Items can be given specific grid properties.

1. Grid Track - Space between two grid lines.
2. Grid Area - Area inside a grid.

## Code Example 1
```
<title>CSS Grid</title>
    <style>
      .container {
        border: 2px solid rgb(255, 145, 0);
        display: grid;
        grid-template-columns: [first]120px [second]100px;
        grid-template-rows: 100px 100px 100px;
      }
      .items {
        border: 2px solid red;
        height: 55px;
        width: 55px;
      }
      .item-4 {
        grid-row: 1/2;
        grid-column: 1/2;
      }
      .item-1 {
        grid-row: 1/2;
        grid-column: 1/2;
      }
    </style>
  </head>
  <body>
    <div class="container">
      <div class="items item-1">1</div>
      <div class="items">2</div>
      <div class="items">3</div>
      <div class="items item-4">4</div>
      <div class="items">5</div>
    </div>
  </body>
```
## Output 1
![image](https://github.com/user-attachments/assets/165eda20-fbae-4989-9131-8171e1f48e5c)

## Code Example 2
```
<title>CSS Grid</title>
    <style>
        .container{
            border: 2px solid black;
            display: grid;
            grid-template-areas: "nav nav nav"
                                "side element element"
                                "footer footer footer";                                   
        }
        .items{
            height: 50px;
            /* width: 50px; */
            border: 2px solid red;
        }
        .item-1{
            grid-area: nav;
            background-color:wheat;
        }
        .item-2{
            grid-area: side;
            background-color:brown;
        }
        .item-3{
            grid-area: element;
            background-color:yellowgreen;
        }
        .item-4{
            grid-area: footer;
            background-color:palevioletred;
        }
        .item-5{
            grid-area: nav;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="items item-1">1</div>
        <div class="items item-2">2</div>
        <div class="items item-3">3</div>
        <div class="items item-4">4</div>
        <div class="items item-5">5</div>
    </div>
</body>
```
## Output 2
![image](https://github.com/user-attachments/assets/17fe695d-7cea-4886-9092-510e2bd25683)

