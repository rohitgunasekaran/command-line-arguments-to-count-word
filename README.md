# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
Step 1: Import sys module to use command line arguments.

Step 2: Use the open() by getting the file name with "sys.argv[1]" which
means the first index of given argument

Step 3: Iterate the content of the file using for loop.

Step 4: Split the contents into each line using .split() function.

Step 5:Iterate the list of lines and increment the value of variable (word) each
time.

Step 6: Run the program by giving "python prgm.py EX12.txt" on the
terminal.
## PROGRAM: 
      #program to command-line-arguments-to-count-word
      #Developed by: rohit g
      #RegisterNumber: 212222240083

       import sys

       count = {}

        with open(sys.argv[1], 'r') as f:

        for line in f:

        for word in line.split():

        if word not in count:

         count[word] = 1

         else:

         count[word] += 1

          print(count)

           f.close()


### OUTPUT:![image](https://github.com/rohitgunasekaran/command-line-arguments-to-count-word/assets/119404546/38166fd6-f35c-4f1c-8479-a64503dc30cd)
![image](https://github.com/rohitgunasekaran/command-line-arguments-to-count-word/assets/119404546/a227d7ad-fea4-44b3-8527-92fe9dbc49f4)





## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
