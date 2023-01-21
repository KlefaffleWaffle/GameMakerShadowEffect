# GameMakerShadowEffect

A collection of code and algorithms used to generate a dynamic sprite/shadow effect in the Game Maker enviroment. Every frame, a block object will draw a shadow based on where the sun is. Using the center point of the sun object and the relevant two corners, the game will calculate the lines that define that shadows. Based on the slope, and knowing the shadow will have a quadrilateral shape, we calculate the remaining two points of the shadow, (The first two points being the corner of the block casting). Once all corners have been found, we create the quadrilateral by calling the "draw_triangle()" function that is native to the language. By calling it twice with slightly different inputs, we can create two shaded triangles that appear to be one quadrilateral.

https://user-images.githubusercontent.com/24324829/213828886-4e568e5a-043d-4d29-8bff-5b5f46bf2f6c.mp4

