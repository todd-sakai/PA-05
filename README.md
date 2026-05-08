# PA-05

Huffman Coding
Problem Context

We will add functionality to the Huffman Coding implementation covered in class. More specifically, your code will need to:

Create one Huffman Tree and set of Huffman codes based on the following MESSAGE_KEY: when zombies arrive, quickly fax judge pat.9876543210

Read multiple messages from a file, then compress and decompress each one based on the same set of codes from the MESSAGE_KEY

Display the Huffman Codes generated, then the original, compressed, and decompressed versions of each message

Input

The program input file contains one message per line. For example, the provided message.in contains the following lines:

abc c
MeSSSY,.-+= message*&@$%
Rotgut whiskey's gonna ease my mind Beach towel rests on the dryin' line
You may assume that the input file contains at least one line/message. You may also assume that message(s):

Will not contain newline characters, since newline characters separate messages

May use a mix of upper- and lower-case letters, but all messages should be converted to lower case before compression.

May include characters not present in the Huffman codes

Such characters should be ignored when compressing

Such characters will not be present after decompressing

Output

The output should print the Huffman Codes generated based on the Huffman Tree. Then, for each message, it should print the original, compressed, and decompressed message.

See message.out for the corresponding output for the sample input.

Starter Code

The starter code includes a main() method that you will need to edit. The starter code also includes a working Huffman Tree implementation.You are encouraged to add a debug flag to write custom test cases, see previous programming assignments for inspiration. Make sure to set debug to False when submitting as the grading scripts will pass inputs through stdin.

Take note of the code style used in the starter file. We will apply a similar rubric (see below) when manually assessing code style.

Approach

We recommend using the following steps to complete this assignment:

Note that the same Huffman Codes will be used on all messages, so be sure to add a constant for the MESSAGE_KEY described above.

The Huffman Tree implementation includes a __str__() method for printing.

Do not modify or delete any of the provided methods, unless you want the extra challenge of implementing a Huffman Tree from scratch. Similarly, do not modify the provided priority queue implementation.

Read one message at a time. Feel free to reference past programming assignments for inspiration.

Add and implement compression and decompression methods.

Feel free to add helper methods, such as one to generate a dictionary of codes.

Carefully check your output against the provided sample output for formatting requirements.

Feel free to use an online diff checker or your terminal for ease of comparison. Ask on Ed Discussion if you need help!

Grading

Grading scripts (automated): 70/100 points. The first test case is based on the sample message.in, and additional test cases are based on data that more fully tests different scenarios.

Code review: 30/100 points. TAs will complete a manual code review for each assignment, similar to how a Team Lead would complete a code review in a professional setting. TAs will also complete a technical requirements review in addition to a code style review.

Please refer to the following code style guidelines for this assignment: 15/100 points

Readability: Descriptive variable and method names, no unused code, no commented out code, and proper indentation.

Documentation: One comment per added/modified method describing the input, output, and purpose of the function. Optional additional comments describing high level purpose of each step within a method.

Organization: Lines of code are less than 100 characters long, methods have one primary purpose, logical structure to approach.

Please refer to the following technical requirements for this assignment: 15/100 points

Generated Huffman Tree based on MESSAGE_KEY.

Compressed and decompressed messages based on Huffman Tree (no hardcoded or manually compressed/decompressed solutions allowed).
