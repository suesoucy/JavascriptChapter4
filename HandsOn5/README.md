In this debugging challenge you will debug a program that converts angular measurements between degrees and radians. The formula to convert an angle measured in degrees to radians is as follows:
radians=degrees x pi/180
And the formula to convert radians to degrees is : degrees=radians x 180/pi
The value of pi can be entered with the built in JavaScript constant Math.PI. The code to do the calculations has been entered for you, but you will have to fix the bugs in the program. A preview of the completed page is shown in Figure 4-34. 
1. Use your code editor to open the project04-05_txt.html and project04-05_txt.js  files from the js04 project05 folder. Enter your name and the date in the comment section of each file and save them as project04-05.html and project04-05.js. 
2. Go to the project04-05.html file in your code editor and in the head section add a script element to load the project04-05.js file, deferring the loading of the JavaScript source file until the entire HTML file is loaded. Study the contents of the HTML file and save your changes. 
3. Go to the project04-05.js file in your code editor. At the top of the file, insert a command so that the code is strictly interpreted. 
4. Directly below the command that declares the radians variable, insert a command that writes the radians value to the debugger console in the form, “Radians=radians”.
5. Directly below the command that declares the degrees variable, insert a command that writes the degrees value to the debugger console in the form “Degrees=degrees”. 
6. Save your changes to the file and then load project04-05.html in your web browser.
7. Use the debugger to locate syntax and runtime errors in the code. Fix those errors in your code editor. 
8. Enter 60 in the Angle in Degrees box. The value for the Angle in Radians should be 1.047, but it is not. Locate and fix the logic error that resulted in the incorrect value being calculated. 

