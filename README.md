# The easiest way to make an aimbot
This project was made for educational purposes.
I do not encourage the usage of third party software.

---

## Table of contents
- [Introduction](#intro)
- [Requirements](#req)
- [Logic](#logic)
- [Code example](#code)

---

## <a id="intro"></a>What is an aimbot?
An aimbot will help you in-game by aiming onto your enemy automatically once an enemy entity is visible.

---

## <a id="req"></a>Things you will need
- A way to emulate mouse movements (can be a software but also hardware)
- A way to read colors from screen pretty fast (We call this the `screenreader` for now)
- Code

**Optional:**
- A way to emulate mouse clicks (can be a software but also hardware)

---

## <a id="logic"></a>How it works
- Screenreader checks your screen for the enemy outline color of your choice (purple recommended); once the color is on the screen make your code simulate a mouse movement.

---

## <a id="code"></a>Code example
(Not actual code)

Code should be a loop until process is being killed; Purple must be defined with a color checker because the rgb value varies depending on distance to object 

**General example:**
```js
mouse = Mouse //define mouse here 
purple = //RGB VALUE HERE //define color here

function main() //function to check for enemies and shoot 
{
  screen = //define screen (can be a screenshot or whatever)
  if(pixel(x,y) === purple) //check if screen has color
  {
    mouse.move(x, y); //aim onto enemy
    //mouse.click(); //auto shoot 
  }
}

if(mouse.rightclick.isPressed() == true) //if RC is clicked 
{
  main(); //execute function 
}
```
^^^
Fictive code; **Making an actual aimbot is way harder! This is just an example for understanding!**

Make sure to always write your own code and not to copy from the internet in order to ensure complete functionality.

---

## Liked this project?
Feel free to leave a star 🌟
