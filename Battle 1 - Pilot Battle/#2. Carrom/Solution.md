# Battle #1 - Pilot Battle

## #2. Carrom

### The Code

This is my solution for #1.2. Carrom.

>***Disclaimer** :* <br/>*This is my own solution and might not be the shortest solution. I'm writing a code that can be easily explain for better understanding of the problem.*

```
<div class="container">
  <div class = "box left top"></div>
  <div class = "box right top"></div>
  <div class = "box left bottom"></div>
  <div class = "box right bottom"></div>
</div>
<style>
  body{
    background: #62374e;
    margin: 0;
  }
  .container {
    margin: 50px;
    width: 300px;
    height: 200px;
    position: relative;
  }
  .box {
    width: 50px;
    height: 50px;
    background: #fdc57b;
    position: absolute;
  }
  .top {
    top: 0;
  }
  .right{
    right: 0;
  }
  .bottom{
    bottom: 0;
  }
  .left{
    left: 0;
  }
</style>
```

### Explanation

As usual, reset the default margin and give a background color to our body.
```
body{
    background: #62374e;
    margin: 0;
  }
```

In the upcoming solutions, you might see me using **container(s)** a lot to wrap all the elements. This is mainly for defining the position, and put margin or padding precisely. In this challenge, define the margin on all sides and then calculate the rest of the body as the width and height. Then we set the position to **relative** to make sure that the box element in the nect section will be positioned **absolute** to the container div and not the body element. In the upcoming problems, we are going to use this pattern a lot, where we put position **relative** to the container and position **absolute** on the elements inside it.
```
.container {
    margin: 50px;
    width: 300px;
    height: 200px;
    position: relative;
  }
```

For the boxes we are going to use a div element that has box and numbers as their classes. Define the size of the box and give it the background color. Set the position to absolute, so we can place all the boxes in all four corners of the container.
```
.box {
    width: 50px;
    height: 50px;
    background: #fdc57b;
    position: absolute;
  }
```
***Note:**<br/> If you want to see the border of the container, you can temporarily put this lines on the html.*
```
.container {
    border : 1px solid black;
  }
```

After that we define the top, right, bottom, and left position to zero. And then we put each number classes on the corresponding box.
```
.top {
    top: 0;
  }
  .right{
    right: 0;
  }
  .bottom{
    bottom: 0;
  }
```

***Note** : <br/>You can actually remove/delete the  top and left since everything on default is on the most top left.*
