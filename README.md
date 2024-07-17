
Step #1: Run a Python program
[ ]
message = "hello";
print(message+" world");
hello world
[ ]
x = input("enter your name: ")
y = int(input("enter an int: "))
z = float(input("enter a float: "))
print (x,y,z)
enter your name: Dancun
enter an int: 2
enter a float: 3
Dancun 2 3.0
Step #2: User Input with Conditionals
[ ]
x = input("enter your name: ")
y = int(input("enter an int: "))
z = float(input("enter a float: "))
if x == 'dancun':
    print ('Welcome dancun!')
else:
    print ('Welcome earthling!')
enter your name: dancun
enter an int: 2
enter a float: 4
Welcome dancun!
Step #3: Using Loops
[ ]
for i in range(0, y):
    print(i, z)
    while x != 'dancun':
        x = input("enter your name a second time: ")
        print('Welcome dancun!')
0 4.0
1 4.0
Step #4: Defining Functions
[ ]
#Define and use functions in your script.
def get_name():
    myname = input("enter your name a third time (using quotes): ")
    return myname
name = get_name()
print('Welcome' + name)
def print_one_greater(x):
    print(x + 1)
    print_one_greater(y)
enter your name a third time (using quotes): dancun
Welcomedancun
Step #5: Working with Lists
[ ]
#Implement list usage in your script.
months = ['jan', 'feb', 'mar', 'apr', 'may', 'jun', 'jul', 'aug', 'sep', 'oct', 'nov', 'dec']
for i, month in enumerate(months, start=1):
    print(i, month)
1 jan
2 feb
3 mar
4 apr
5 may
6 jun
7 jul
8 aug
9 sep
10 oct
11 nov
12 dec
Step #6: Utilizing Dictionaries
[ ]
#Utilize dictionaries in your script.
months2 = {'jan': 'January', 'feb': 'Febuary', 'mar': 'March', 'apr': 'April', 'may': 'May', 'jun': 'June','jul': 'July', 'aug': 'August', 'sep': 'September', 'oct': 'October', 'nov': 'November', 'dec': 'December'}
 
# Correct the misspelling of 'February'
months2['feb'] = 'February'
for i, month in enumerate(months, start=1):
    print(i, months2[month])
1 January
2 February
3 March
4 April
5 May
6 June
7 July
8 August
9 September
10 October
11 November
12 December
Step #7: File Input
[ ]
#Create a new dataset file, `data.txt`, with the provided values.

   -1
   0
   1
   2
   3
   4
   5
[ ]
# Read and print the file's content in your script.
filename = "data.txt"
with open(filename) as fin:
    content = fin.read().splitlines()
    print(content)
['-1', '0', '1', '2', '3', '4', '5']
Step #8: File Output
[ ]
#Write the converted Celsius to Fahrenheit values to a new output file, `data2.txt`.
fout = open("data2.txt", "w")
for line in content:
    celsius = float(line)
    fahrenheit = (celsius * 9 / 5) + 32
    fout.write(str(fahrenheit) + "\n")
fout.close()
Step #9: Optional - Celsius to Fahrenheit Converter
[ ]
#Create a new Python program, e.g., `ctof.py`, with the following code to convert Celsius to Fahrenheit one line at a time.
with open("data.txt") as fin:
    for line in fin:
        celsius = float(line)
        fahrenheit = (celsius * 9 / 5) + 32
        print(fahrenheit)
30.2
32.0
33.8
35.6
37.4
39.2
41.0
[ ]

