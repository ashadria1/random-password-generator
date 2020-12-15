# random-password-generator

This application is a simple design for a random password generator in javascript.

Based on the four criteria, a random number is generated to randomly select a criteria to choose from.

Then, a random number is generated to select a random element from that array, incrementing the character count each time.

Repeat until the character count is equal to the user defined password length.

Then, concatenate the resulting characters into a final string.

Criteria:
GIVEN I need a new, secure password
WHEN I click the button to generate a password
THEN I am presented with a series of prompts for password criteria
WHEN prompted for password criteria
THEN I select which criteria to include in the password
WHEN prompted for the length of the password
THEN I choose a length of at least 8 characters and no more than 128 characters
WHEN prompted for character types to include in the password
THEN I choose lowercase, uppercase, numeric, and/or special characters
WHEN I answer each prompt
THEN my input should be validated and at least one character type should be selected
WHEN all prompts are answered
THEN a password is generated that matches the selected criteria
WHEN the password is generated
THEN the password is either displayed in an alert or written to the page

I was able to generate random numbers with no problem, but apparently am missing something in the syntax to make my if-else statements work. Instead of grabbing an array at random, it seemed to either go through all four criteria, or only one, depending on what code I used.

The incrementing of the character count was supposed to keep pace with the selection of a character, but for some reason changes depending on whether I use multiple if statements vs. if-else statements.

Else-if seems to generate random numbers fine, but pulls all characters from one array.

If seems to generate random numbers fine, but pulls from all arrays equally, and in succession. I hope to figure this one out.

I was not able to concatenate the characters as of the time of this submission, but hope to add it in the future.

I was able to write all values to the console.

The link to the deployed site is:
https://ashadria1.github.io/random-password-generator/

Here is a screenshot of the application in action:
assets\PwdGenscreenshot2.PNG
