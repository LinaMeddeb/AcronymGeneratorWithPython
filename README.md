# AcronymGeneratorWithPython
In this tutorial, you'll learn to create a simple Acronym Generator using Python.

What is an Acronym?
An acronym is a word formed by abbreviating a phrase by combining certain letters of words* in the phrase (often the first initial of each) into a single term.
*'of' is not considered for acronyms

.How our Acronym generator works?
Our Acronym Generator will take a String as an input and for the output it will return the initials of all the words in the String.




Let's start coding!
Step 1: Getting the user input.
First of all, we need to get the phrase from the user.
We can do it easily with the use of input() method, the user input will be stored in an input_user variable.

#adding the user input
input_user = input("Please Tape a phrase: ")

Step 2: Ignoring 'of'
In the second step, we have to ignore ‘of’ from the user input .
#ignore 'of'
clean_input = (input_user.replace('of', ''))

Step 3: Creating a list of words
Next step,  we need to extract the words from the  clean_input string and to store them as a list in phrase variable.
# Split words
phrase = clean_input.split()

Step 4: Coding the acronym generator's logic
Then, we initilize an empty variable acronym .
acronym = ""
we are going to extract the first letter of every word stored in phrase using slicing operator and adding it to acronym variable than capitalizing it with the use of upper() function. .
for w in phrase:
    acronym = acronym + w[0].upper()
Finally, Let's add a print statement
print('The acronyme of ' + input_user + ' is '+ acronym)
Final Step: Running the code
let's try running our Code!
