

# New122 
1.	   Write down an algorithm that reads in a positive integer x and tests if it is a prime number.

Note: (1) A number is prime if it is only divisible by 1 and itself.

(2) The integer 1 is defined as non-prime.

      Solution :

1.	Input: Positive integer x.

2.	Special Case Handling:

o	If x is less than or equal to 1, output "Not prime" and terminate the algorithm because 1 is not considered a prime number.

3.	Check for Divisibility:

o	Loop through potential divisors i from 2 to x−1:

	If x is divisible by i (i.e., xmod  i=), then x is not a prime number. Output "Not prime" and terminate the algorithm.

4.	Prime Determination:

o	If no divisors are found in the previous step (i.e., x is not divisible by any number in the range from 2 to x−1), then x is a prime number. Output "Prime".





2.	     Write down an algorithm to find out smallest and largest amongst 3 elements.

       Solution :

           Input: Three integers a, b, and c.

          Initialization:

•	 Assume a as the initial smallest and largest value.

•	This assumption simplifies the comparison process.

          Comparison Process:

•	Compare b with the current smallest and largest values:

o	If b is smaller than the current smallest, update the smallest value to b.

o	If b is larger than the current largest, update the largest value to b.

•	Compare c with the current smallest and largest values:

o	If c is smaller than the current smallest, update the smallest value to c.

o	If c is larger than the current largest, update the largest value to c.

          Output:

•	             After comparing all three elements a, b, and  c, the updated smallest and largest values will  give you the smallest and largest among the three elements.











3)         Modify the above algorithm so that it will work with N elements where N is accepted from the user.

Solution : 

          Input: An array arr of N integers.

         Initialization:

Assume the first element arr[0] as the initial smallest and largest value.

         Comparison Process:

•	     Iterate through the array from index 1 to N−1:

                                  Compare each element with the current smallest and largest values:

	If the element is smaller than the current smallest, update the smallest value.

	If the element is larger than the current largest, update the largest value.

         Output:

                   After iterating through all elements, the updated smallest and largest values will give you the smallest and largest among the N elements.

 



4)           Write down an algorithm to read in an integer between 0 and 99 and output the value in

               English. For example, if the input is 28, it should output “twenty-eight”.



Solution :

              Step 1: Define arrays or lists to hold the English words for numbers 0-19 and multiples of ten (20, 30, ..., 90).

               Step 2: Determine the tens and units digits of the input number n.

•	If n is less than 20, use the direct word from the array for numbers 0-19.

•	For numbers 20 and above, use the array for multiples of ten (20, 30, ..., 90) and append the word for the units place if it's not zero.

              Step 3: Construct the output string based on the tens and units places determined in Step 2.















5)          Write down an algorithm to get the weight (in kilograms) and height (in meters) of a person.

                  Then calculate and print the Body Mass Index (BMI) according to the formula:

                                          BMI = weight / (height*height)

                      The BMI should be printed with 3 decimal places. You should choose an appropriate data types and names for your variables. 



Solution : 

           Input:

•	Read the weight weight_kg in kilograms.

•	Read the height height_m in meters.

          Calculate BMI

•	Compute the BMI using the formula: 

                                                  BMI= (weight_kg / height_m^2)

          Output:

•	         Print the BMI with 3 decimal places.





6)         Write down an algorithm to read in a temperature in Celsius and convert it to Fahrenheit. The

             relationship between Celsius and Fahrenheit is  C = (F-32)*5/9.



Solution :

           Input:

•	Read the temperature temp_celsius  in Celsius.

         Conversion Formula:

•	Calculate the temperature in Fahrenheit using the formula:   

                  Temp_fahrenheit =  (temp_celsius × (9/5) + 32)

        Output:

•	 Print the temperature in Fahrenheit.







7)    Write down an algorithm to find out roots of a quadratic equation. Please note that roots can

 be imaginary.

     Solution : 

             Input:  Coefficients a, b, and c of the quadratic equation ax^2+bx+c=0.

            Calculate Discriminant:

           Compute the discriminant Δ=b^2−4ac

           Determine Root Type:

•	If Δ>0: Two distinct real roots.

                                   Calculate two real roots: 

                                                  X1= (-b+√ Δ) / 2a                  X2= (-b-√ Δ) / 2a

                                           Output x1 and x2

•	  If Δ=0: One real root (repeated).

                               x1=x2= -b/(2a)

                          Output  x1

•	If Δ<0: Two complex roots (imaginary).

                                            Calculate two complex roots:

•	Real part:

                                                            Real_part = -b/2a

•	Imaginary part:

                                       imag_part = √ |Δ| / (2a)



•	Output the roots in the form:         

                  x1=real_part + imag_parti,   x2 = real_part−imag_parti 



•	Output: Display the roots based on the calculations in steps 3.







8.   Write down an algorithm that reads in the number of seconds and converts it to hours, minutes and seconds. A sample output of your program is as follows. Don’t bother with the singular or plural forms of the nouns.

Solution :

             Input:   Receive the number of seconds total_seconds

            Calculate Hours, Minutes, and Seconds:

                                  Compute hours             :         hours  = (total_seconds/3600)

                                  Update total_seconds   :         total_seconds  = total_seconds mod /3600

                                  Compute minutes         :         minutes = total_seconds / 60

                                  Compute remaining seconds     :          seconds   =   total_seconds mod  60 

        

            Output  :    Display the result in the format   :

                                                       total_seconds seconds = hours hours minutes minutes seconds seconds





 9.      Write down an algorithm that reads in a mark of a student (which is an integer between 0 and

         100 and prints the corresponding grades (A-F). The mark-to-grade conversion table is as follows:

                  Grade:    A            B         C        D            F

                 Range:     ≥80     65-79   50-64    40-49     <40



1. Modify the program to allow user-specified grade boundaries. You may need to define more variables.

2. Modify the program so that it checks if the input is between 0 and 100. If not, it should ask the user to input again until the input is in the correct range. Use while statements.

3. Modify the program so that it repeats the above computation on 50 students. Use while statements.











Solution :    

            Part 1: Convert a Mark to a Grade

1.	Input: Receive a mark from the user (an integer between 0 and 100).

2.	Check Input Range:

                 Ensure the mark is between 0 and 100. If not, inform the user and ask for input again.

3.	Determine Grade:

                    Using conditional statements, assign a grade based on the mark according to the table provided:

	Grade A: ≥80

	Grade B: 65−79

	Grade C: 50−64

	Grade D: 40−49

	Grade F: <40

4.	Output: Display the corresponding grade.

       Part 2 : Modify to Allow User-Specified Grade Boundaries

1.	Input: Receive marks and user-defined grade boundaries (as integers).

2.	Check Input Range:

o	Ensure the mark is between 0 and 100. If not, ask for input again.

3.	Determine Grade:

o	Use conditional statements with the user-specified boundaries to assign grades.

4.	 Output: Display the corresponding grade.



      Part 3: Modify to Repeat Computation for 50 Students

1.	Initialize Counter: Set i=1 (to count up to 50 students).

2.	Repeat Loop: Repeat the following steps until iii reaches 50:

o	 Input: Receive mark from the user.

o	 Validate Input: Ensure the mark is between 0 and 100 using a while loop.

o	Determine Grade: Use conditional statements to assign the grade based on the mark.

o	Output: Display the mark and corresponding grade.

o	Increment Counter i















10 . Write down an algorithm which will perform following functionality

Read an integer array

Display above array

Find out sum of all elements of an array

Find out mean of an array

Find out standard deviation of an array

Find out probability of occurrence of every element in an array

Draw histogram



Solution : 

          •  Input: Receive an integer array array\text{array}array.

•  Display Array:

•	Output the elements of array.

•  Calculate Sum of Array Elements:

•	Initialize sum to 0.

•	Traverse through each element  in array and add element to sum

         •  Calculate Mean of Array:

•	Compute the mean using the formula :

                        Mean = sum/length of array

•	Calculate Standard Deviation of Array:

•	Initialize sum_squared_diff  to 0.

•	Traverse through each element in array and compute squared differences from the mean.

•	Compute standard deviation std_dev using the formula:

                                         Std_dev = √(sum_squared_diff)/(length of array)

•	Calculate Probability of Occurrence:

•	Create a dictionary prob_dict to store frequencies of each element.

•	Traverse through each element in array:

o	If element is not in prob_dict , initialize it with a count of 1.

o	If element is already in prob_dict, increment its count.

•	Calculate probability for each unique element as :

                                      Probability(elements) = (count of element) / (length of array)

•  Draw Histogram:

•	Use a plotting library or tool to visualize the frequency of each element in array.

•  Output:

•	Display the sum, mean, standard deviation, and probability of occurrence for each element.

•	Display or draw the histogram.











 

                            





              

