# RubricPortrait
## Rubric cube portrait builder
![](/img/ex1.png)

## General Workflow
The program is executable only in the jupyter file Rubric Portrait.ipynb. Once in the notebook, users will have to copy paste the image path to the varaible imgPath (The image needs to be in .png file) and then identify the amount of rubric cubes, 96(small) 150(medium) 600(large), that the users will be using in the variable rubricCubes. Obviously, the fewer number of cubes used, the harder it is to make sense of the portrait. Image below are examples and differences between the 3 different sizes.
![](/img/ex2.png)

Additionally, users may use the command step() for a step-by-step instruction to easily follow and build the portrait with rubric cubes. 

## Method
What the program does is that it will draw any imported image with the 6 colors of a rubric cube. The program will loop through each image pixel and replace it with one of the 6 rubric cube colors. In order to know which pixel be replaced with which color, the imported image will first have to turn into a grayscale image,  extract the grayscale value (ranging from 0 to 255) for each pixel, then replace that pixel with the color according to the scale below. 
![](/img/ex3.png)

Notice that the color green is not used because according to the color theory, green does not blend well with the other 5 colors when building a portrait.

## Limitation
Although the program can draw any image with rubric cubes, if the person/object in the picture is too small or the color of the person/object is similar to the background (lack of variety of colors in the original image), then the result may not be favorable even with 600 cubes.

![](/img/ex4.png)