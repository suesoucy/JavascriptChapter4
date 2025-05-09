In a comment text box, reviewers are often given a character limit that they cannot exceed. In this project, you will debug the code for an application that counts the number of characters in a posted comment to ensure the comment does not exceed a predetermined limit. The app makes use of the keyup event which is triggered when a key is pressed and then released up from the keyboard as part of typing a character. A function named countCharacters() has been provided that counts the characters in review. Your job will be to locate and fix the errors in the code and to catch user error when the review exceeds the character count limit. A preview of the page for a character count limit of 100 is shown in figure 4-32. 

1. Use your code editor to open the project04-03_txt.html and project04-03_txt.js files from the js04 project04 folder. Enter your name and the date in the comment section of each file and save them as project04-03.html and project04-03.js.
2. Go to the project04-03.html file in your code editor and in the head section add a script element to load the project04-03.js file, deferring the loading of the JavaScript source file under the entire HTML file is loaded. Study the contents of the HTML file and save your changes. 
3. Go to the project04-03.js file in your code editor. At the top of the file, insert a statement directing that the code be interpreted under strict standards.
4. Go to the updateCount() function. Insert at the bottom of the function a try catch finally statement that does the following
   
    - Within the try statement, test if the chartCount variable is greater than the value of the MAX_REVIEW constant. If it is, throw an exception with the error message “You have exceeded the character count limit.”
    - For caught exceptions, display the error message within the innerHTML of the warningBox object. 
    - Whether the exception is thrown or not, change the innerHTML of the wordcountBox object to the value of the chartCount variable.
6. Save your changes to the file and then load project04-03.html in your web browser. Start typing text into the comment box.
7. There are several errors within the code. Use the debugger to find any syntax or runtime errors you encounter. Fix the errors in your code editor. 
8. When the app is free of errors, attempt to type more than 100 characters into the comment box. Verify that when you exceed the character limit, a warning message appears on the page. 
9. Return to your code editor and increase the value of MAX_COUNT from 100 to 1000.

