# Hell Let Loose Calculator

![forthebadge](https://forthebadge.com/images/badges/uses-js.svg)
![forthebadge](https://forthebadge.com/images/badges/built-with-grammas-recipe.svg)

![](https://i.imgur.com/IyOzgnk.jpeg)

**Based on the project by [@pastuh](https://github.com/pastuh): [hllminicalculator](https://pastuh.github.io/hllminicalculator/)**

## Linear Regression

In-game table:

![](https://i.imgur.com/kL1Krhs.png) 

As we can see, here is a linear dependence:

![](https://i.imgur.com/KOkynQU.png)

So we can use linear regression

```
Sum of X = 13600
Sum of Y = 12800
Mean X = 850
Mean Y = 800
Sum of squares (SSX) = 3400000
Sum of products (SP) = -806100

Regression Equation = ŷ = bX + a

b = SP/SSX = -806100/3400000 = -0.23709

a = MY - bMX = 800 - (-0.24*850) = 1001.525

ŷ = -0.23709X + 1001.525
```

MIL calculation method:

```js
let m = -0.23709;
let b = 1001.525;

let distanceResult = (100 * input) / 1600;
let calculated = m * input + b ;
let realResult = Math.round( calculated * 10) / 10;
```
