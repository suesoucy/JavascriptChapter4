In this project you will work with an app that calculates the change returned for a purchase and breaks down the amount in units of currency from pennies up to $20 bills. However, there are errors in the code that must be corrected. A preview of the completed page is shown in figure4-33. 
1. Use your code editor to open the project04-04_txt.html and project04-04_txt.js files from the js04 project04 folder. Enter your name and date in the comment section of each file and save them as project04-04.html and project04-04.js.
2. Go to the project04-04.html file in your code editor and in the head section add a script element to load the project04-04.js file, deferring the loading of the JavaScript source file until the entire HTML file is loaded. Take some time to study the contents of the file, paying special attention to the ids of different elements in the page. Save your changes to the file. 
3. Go to the project04-04.js file in your code editor. At the top of the file insert a command so that the code in the file is interpreted with strict adherence to the JavaScript standards for syntax. 
4. Study the contents of the file, noting the different functions that are used to create the challenge calculator. Save your changes to the file. 
5. Open the project04-04.html file in your web browser. To run the program, enter a cash value in the Cash Amount box and the bill in the Bill box. An event handler should calculate the change in response to those events. There are serval syntax and runtime errors in the program. Use the debugger to assist you in locating the errors. Use your code editor to fix the errors you find. 
6. Once the program operates without syntax or runtime errors, use it to calculate the change from $20 for a bill of $12.31. While the change is correctly calculated, the breakdown in units of currency is not. Use the tracing features of the debugger to trace the error to its source. Use your code editor to fix the problem. When the program works as intended, the change and currency amounts should match that shown in Figure 4-33. 
7. Return to the project04-04.js in your code editor. If the bill is greater than the cash amount, no change can be given. Handle this user error by adding a try catch statement to the runTheRegister() function. Within the try catch statement do the following: 
    - Within the try statement test if changeValue is not greater than or equal to zero. If that condition is true, throw an exception with the error message “Cash amount doesn’t cover the bill.”
    - Run the following commands;
changeBox.value = formatCurrency(changeValue):
calcChange (changeValue):
    - Within the catch statement set the innerHTML of the element with the id “warning” to the value of the thrown exception. 
8. Save your changes to the file. Reload project04-04.html in your browser. Verify that if the Bill value is greater than the Cash Amount value, no calculator is done on the change and a warning message appears on the page. 

