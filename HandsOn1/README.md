In this project you will finish an application that provides a general estimate of costs from a moving company. The company charges .50 cents per pound of items moved and .75 cents per mile plus an optional $500 fee for setting and installing furniture and appliances. The program code needs some debugging work and extra code to account for user error. A preview of the completed page is shown in figure 4-30. 

1. Use your code editor to open the project04-01_txt.hmtl and project04-01_txt.js files from the js04 project01 folder. Enter your name and the date in the comment section of each file and save them as project04-01.html and project04-01.js. 
2. Go to the project04-01.html file in your code editor and in the head section add a script element to load the project04-01.js file, deferring the loading of the program until the web page finishes loading. Study the contents of the HTML to become family with the elements and the ids associated with each element. Save your changes to the file. 
3. Go to the project04-01.js file in your code editor. At the top of the file above the comment section, insert a statement that indicates this program adheres to a strict interpretation of JavaScript syntax. 
4. There are two logic errors in setting up the global constants. Locate and fix those errors. 
5. Go to calcTotal() function. To guard against users entering a zero or a negative value for the estimated weight, place the statement totalCost += wgtBox.value * COST_PER_LB; with a try catch statement that does the following

     - Tests whether wgtBox.value is not greater than 0 by using the expression ! (wgtBox.Value > 0). If that expression is true, throw an exception with the error message “!! Enter a positive weight”

    - If no exception is thrown then run the command totalCost +=wgtBox.value * COST_PER_LB;.
   
    - If an exception is caught, set the value of msgBox.innerHTML to the error message you defined for the thrown exception.
   
7. Repeat Step 5, for the estimated distance cost using distBox.value. Throw the error message “!! Enter a positive milage” for a caught exception. 
8. Save your changes to the file. 
9. Open project04-01.html file in your web browser/ Open the debugger and confirm that there are no syntax errors. If there are, fix your code in your code editor. 
10. Test your code by entering 0 for the estimated weight and 1200 for the mileage. Confirm that the error message “!! Enter a positive weight” appears next to the total box. 
11. Change the weight to 2500 and enter a 0 for the estimated mileage. Confirm that the error message “!!positive mileage” appears next to the total box.
12. Enter a milage of 1200 miles and click the Setup and Installation box. Confirm that the estimated moving cost is calculated to be $2650. 

