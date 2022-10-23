-----------------------------------------------------------------------------------------------------------------------------	
				              c++ Computer Science – 1
-----------------------------------------------------------------------------------------------------------------------------


This repository is a collection of c++ program assignments from COSC 1030 - Computer Science-1 class at Laramie County Community College.
Related links:
https://www.lccc.wy.edu
https://lccc.wy.edu/pathways/sciTechEngMath/computerScienceProgram/index.aspx

-----------------------------------------------------------------------------------------------------------------------------
COSC 1030 – Computer Science 1
Professor: David Durbin
Fall Semester - 2022
Student: Alejandro (Alex) Ricciardi

-----------------------------------------------------------------------------------------------------------------------------

Map description:
The programs are stored in folders named after the corresponding assignment; folders can contain one or more programs. 
The folder’s names number that precedes the assignment name is a chronologic reference, 
with the letter ‘12’ representing the oldest assignment, containing the first assignment.

-----------------------------------------------------------------------------------------------------------------------------

Requirement:
c++ 11 or later
I used MS Visiual Studio IDE to creat my programs


-----------------------------------------------------------------------------------------------------------------------------
					           Assignements
-----------------------------------------------------------------------------------------------------------------------------

----------------
7_array_vector
----------------

Complete the following programs; 
when finished take a screen capture of the output from your running program and package it with your .cpp file. 
Submit your work in a zipped folder.
Yes, you need to do all four of these. Two are about vectors and two are about arrays. Make sure you use the correct type for each program.

1. Full Moons

Using the data provided below, create a program that stores the dates of the full moons for the rest of 2022 in a integer array.  
Have the user enter the current date.
and return the number of days until the next full moon. Full moon information can be found at THISLinks to an external site. web page.  
If the user enters a date that is past the full moon for the current month the program should move to the next month. 
If the user enters a date after December 18th the program should return an error message.

INPUT VALIDATION:  
Do not accept numbers above 31 as the day for the date in March, May, July, August, October or December 
and do not accept a number above 30 for April, June, September or November.  Do not accept a number below 10 or above 12 for the month.

Hint: 
You don't have to use the date entered by the user! (You do still need the user to enter the date though.) 
If you #include <ctime> you can get the current date from the system clock! Search for ctime and getdate() for c++.

2. Get and Display Names

Ask the user for a first name and store it in a vector of strings. 
Do this 10 times.  After the final name, print the names to the screen in reverse order of entry.  
Then do this with a second set of 10 names using a character array. The amount of space allocated for each name should be at least 15 characters. 
(REMEMBER: The final place in an array holds the null terminator; this is not counted as a character!)

3. Revisiting: RNG and You

Flip a coin 500 times and store the information in a vector. Using a for loop, 
get the number of heads flipped and subtract this from the total size of the vector using size().  
Roll two 6-sided dice 1000 times and record the number of times each combination of numbers (2-12) is rolled.  
Display these to the screen with proper labels and spacing.
(Yes, you can just modify your existing code rather than writing it all from scratch. Make sure you get your numbers correct though.)

4. Driver's License Exam

The local Driver's License Office has asked you to write a program that grades the written section of the drive's license exam.  
The exam has 20 multiple choice questions; the correct answers are below:
1. B   2. D   3. A   4. A   5. C   6. A   7. B   8. A   9. C   10. D  
11. B   12. C   13. D   14. A  15. D   16. C  17. C   18. B   19. D   20. A
Your program should store the correct answers (show above) in an array.  
It should ask the user to enter the student's answers for each of the 20 questions and store the answers in a second array.  
After the student answers have been entered, the program should display a message indicating whether the student passed or failed the exam.  
(At least 15 correct answers are required to pass the exam.)  The program should then display the total number of correctly answered questions, 
and a list showing the question numbers of the questions the student got wrong. 

Input Validation: 
Only accept the letters 'A', 'B', 'C' and 'D' as answers.

Note that there is now a criteria in the grading for your comments in the program.  
You need to start commenting about what things do, 
where variables are being used (especially if you are passing them to functions) and your loops/conditionals. 
Switch statements are conditionals. Purposes of functions. I won't be jumping on you hard over this (yet). 
But I will be leaving comments in the rubric for your submissions, so make sure you check that. 
(If you want a sample, look at the paintJobEstimator_Sample file in module 6.) 
Larger programs with longer and more complex loops or conditionals would need more detailed comments around those items, 
and comments for functions as well. 
Functions should have at least a minimal comment detailing what the purpose of the function is.

-----------------------------------------------------------------------------------------------------------------------------

----------------
8_functions
----------------

Complete the following programs; take screen captures of your output, package them with your .cpp source files and submit in a zipped folder.

1. Celsius Temperature Table

The formula to convert a temperature from Fahrenheit to Celsius is:
C = (F - 32) * 5/9   < With F being the Fahrenheit temp and C being the Celsius temp.>
Write a function called Celsius that accepts the Fahrenheit temperature as an argument. 
 The function should return the temperature after it has been converted to Celsius.  
Demonstrate the function by putting it in a loop that displays first the Fahrenheit temperature 
and then the Celsius equivalent temperature every 6 degrees between 32 degrees Fahrenheit and 92 degrees Fahrenheit.  
Use proper headings and spacing to make the output easy to read.

2. Winning Sales Division

Write a program that determines which of a company's eight divisions 
(Northeast, Southeast, NorthCentral, SouthCentral, NorthPlains, SouthPlains, Northwest, Southwest) 
had the greatest sales for a quarter. The program should include the following two functions, both of which will be called by main.
double getSales( ) is passed the name of a division; 
it will ask the user for a division's quarterly sales figure, validate that input, then return it. 
This function should be called once for each division.
void findHighest( ) is passed all eight sales totals.  
It will determine which is the largest and print the name of the corresponding sales division and sales figure.

INPUT VALIDATION: 
Do not accept values lower than $0.01 for the sales figure.

3. Paint Job Estimator

A painting contractor has determined that for every 115 square feet of wall space, 1 gallon of paint and 6 hours of labor will be required.  
The company charges $54.00 per hour for labor.  
Write a modular program that allows the user to enter the number of rooms to be painted, the price of paint per gallon, 
and then the square footage of each room.  The program should then display the following information properly spaced and labelled:

- The number of gallons of paint required.
- The total hours of labor needed. (This is a union job, so assume they'll be taking breaks and not working more than 10 hours per day. 
Divide up into working days if necessary.)
- The total cost of the paint.
- The labor charges.
-The total cost of the paint job.

INPUT VALIDATION: 
Do not accept a value lower than 1 for the number of rooms; all rooms must have at least 85 square feet of wall space to be painted. 
The average cost of the paint is $32.50 per gallon, do not accept values lower 75% of that price or greater than 1.25 times that price. 

-----------------------------------------------------------------------------------------------------------------------------

----------------
9_loops
----------------

Complete the following programs; when finished take a screen capture of the output from your running program and package it with your .cpp file. 
Submit a zipped folder with your work.

1. Hotel Occupancy

Write a program that calculates the occupancy rate for a hotel; 
the program should start by asking the user for the number of floors in the hotel.  
A for loop should then iterate once for each floor.  In each iteration, 
the loop should ask the user for the number of rooms on the floor and how many of them are occupied.  After all the iterations, 
the program should display how many rooms the hotel has, how many of them are occupied, how many are unoccupied, 
and the percentage of rooms that are occupied. 
The percentage may be calculated by dividing the number of occupied rooms by the total number of rooms.

NOTE: It is traditional that no hotel have a 13th floor!  The loop should skip the entire 13th iteration.

INPUT VALIDATION:  
Do not accept values less than 13 for the number of floors.  
Do not accept a number less than 10 or greater than 24 for the number of rooms per floor.

2.  Random Number Guessing Game

Write a program that generates a random number between 1 and 100 and asks the user to guess what the number is.  
If the user's guess is higher than the random number, the program should display "Too high, try again."  
If the user's guess is lower than the random number the program should display "Too low, try again."  
The program should use a do-while loop that repeats until the user guesses the number correctly.  
The program should also employ a while loop that keeps track of the number of guesses made by the user and, 
once the user guesses the number correctly, displays the number of guesses the user made.

-----------------------------------------------------------------------------------------------------------------------------

----------------
10_rng_and_you
----------------

Using the random number generation that was covered in class, create the following programs:

1. Flip a coin 50 times 
and get the number of heads flipped and the number of tails flipped.  
Roll two 6-sided dice 50 times and record the number of times each combination of numbers (2-12) is rolled.  
Display these to the screen with proper labels and spacing.  

2. A Battleship game board is 10 x 10. 
The PT Boat holds 2 pegs, the submarine and Frigate hold 3, the Battleship 4 and the Aircraft carrier 5.  
Based on this information, use random numbers to figure out the average number of turns 
it will take to sink all five ships over 5 games of Battleship.

Place your screen captures and .cpp files in a folder, zip that folder and submit it.

Hints:

1. This isn't as complicated as it looks, so don't try to make it more complicated than it is.

2. Get a random number between 0 & 1 (see sample program). Track the number of 0's and number of 1's. Do that 50 times.  
Use a switch statement for the dice. (See week 3's menu template for an example of a switch statement.)

3. 10 * 10 == 100.  2+3+3+4+5 == 17.  Get a random number between 1-100 (0-99, don't forget the computer starts at 0!) 
And if that number is between 1 and 17 (0-16) you hit a ship. Each time you get a new random number is 1 turn. Record number of turns. 
Repeat until you get 17 hits. Repeat that process 5 times.  Take the average.
Yes, it will be a long program. Copy/Paste is your friend (make sure the code works before you copy/paste).

4. Have a good weekend.
5. You can use loops if you want.

-----------------------------------------------------------------------------------------------------------------------------

----------------
11_conditionals
----------------

This is a two part assignment: Part 1 consists of creating a flowchart diagram; part 2 will be writing a program to match that diagram.

Part 1:  Create a flowchart using the tools in the Useful Resources module of how you should dress based on the following weather conditions: 
Temperature over 80 degrees Fahrenheit (temp>80); 
Temperature over 50 degrees Fahrenheit (temp<80 &&temp>50); 
Temperature below 32 degrees Fahrenheit (temp<32); Raining (note that if the temperature is below 32 degrees Fahrenheit 
and it is raining then we consider that to be snowing). 
The check for rain can be a simple yes or no ('y' or 'n').

Part 2: Based on your flowchart, create a C++ program that follows the same process. 
You will need to use conditional statements for this program. 

When the program is complete, run the program 2 times with different criteria, 
take screen captures of BOTH sets of results! (You should be asking the user for the temperature and whether or not it is raining.)

Package your screen captures, flowchart and .cpp file into a zipped folder and turn that in.

-----------------------------------------------------------------------------------------------------------------------------

----------------
12_math
----------------

1. Box Office

A movie theater only keeps a percentage of the revenue earned from ticket sales, the rest of the money goes to the movie distributor.  
Write a program that calculates the theater's gross (overall amount earned) 
and net (amount after the distributor's cut) box office profit for one night.  
The program should ask for the name of the movie and how many adult tickets and child tickets were sold.  
Adult tickets cost $12.00 each; seniors and children tickets cost $9.00 each. Students and Military with valid ID are $10.00 each.  
The theater keeps 20% of the ticket sales, the remainder goes to the distributor.  
Have the program display the information in the same format as the example below:

Movie Name:                     " Movie Name "
Adult Tickets Sold:                 ##
Senior/Child Tickets Sold:          ##
Student/Military Tickets Sold:      ##
Gross Box Office Profit:          $ ###.##
Net Box Office Profit:            $ ###.##
Amount Paid to Distributor:       $ ###.##
When finished, take a screen capture of your output and submit both the screen capture and your .cpp file in a zipped folder.

2. Monthly Payments

The monthly payment on a loan may be calculated with the following formula:
Payment = ((Rate * (1 + Rate) ^ N) / (((1 + Rate) ^ N) - 1)) * L     <- Note that no parenthesis comes after L!

Rate is the monthly interest rate, which is the annual interest rate divided by 12. N is the number of payments, 
and L is the amount of the loan. Write a program that asks for these values and displays a report similar to the following example:

Loan Amount:                       $ 10000.00
Annual Interest Rate:                 12%
Monthly Interest Rate:                 1%
Number of Payments:                   36
Monthly Payment:                   $ 332.14
Interest Paid:                     $ 1957.15
Total Amount Paid:                 $ 11957.15

DO NOT use the same numbers I did!  
When finished, take a screen capture of your output and submit both the screen capture and your .cpp file in a zipped folder.

-----------------------------------------------------------------------------------------------------------------------------
