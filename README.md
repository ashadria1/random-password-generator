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

First, I generated a random number between 1 and 4, corresponding to the four different criteria (lowercase, uppercase, numbers, and special characters).  If they selected that particular criteria, a random number was then generated to pull a random element from that particular array, and then incrementing that individual criteria choice count.  If not, it moves to the next if statement to see if that criteria is met (whether or not they selected that criteria).

At first, I was able to generate random numbers between 1 and 4 with no problem, but was apparently missing something in the syntax and/or logic that prevented my if-else statements from working. Instead of grabbing an array at random, it seemed to either go through all four criteria equally, or only one criteria, depending on what code I used (if or if else, etc.), until or before it reached the length of the user defined password. 

As it turns out, the incrementing of the character choice count had to be separated from the total sum of all individual character choices, so that the function would run until the total number of individual criteria character counts equal the length of the user defined password, and not the ATTEMPTS to find a character that fits the criteria, or the character choice count.

I also needed to update my syntax to "===" instead of "=" to make my logic work.

I was able to concatenate the characters by using the document write() function, which automatically concatenates the characters.

I was able to write all steps and values to the console.

The link to the deployed site is:
https://ashadria1.github.io/random-password-generator/

Here is a screenshot of the application in action:
assets\PwdGenscreenshot2.PNG
