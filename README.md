This program reads data from a CSV file containing pizza menu information and displays it as a formatted table in the terminal.
It uses Python’s built-in csv module to parse the file and the tabulate library to present the data in a readable grid format.

The program is run from the command line and requires exactly one argument: the name of a CSV file.

How It Works

The program checks that exactly one command-line argument is provided.

It verifies that the argument refers to a file with a .csv extension.

If the file does not exist, the program exits with an error message.

The CSV file is read using csv.DictReader.

Each row is stored as a dictionary.

The data is printed as a formatted table using tabulate.

How to Run

Make sure you have Python 3 installed and the tabulate library available.

Install tabulate if needed:

pip install tabulate


Run the program from the terminal:

python pizza.py menu.csv


Example:

python pizza.py pizza.csv


Output:

+----------+--------+-------+
| Regular  | Small  | Large |
+----------+--------+-------+
| Cheese   | $13.50 | $18.95|
| 1 topping| $14.75 | $20.95|
+----------+--------+-------+

Error Handling

The program exits with an appropriate message in the following cases:

No command-line argument provided

More than one command-line argument provided

File is not a CSV file

File does not exist

Concepts Used

Command-line arguments (sys.argv)

CSV file handling

Dictionaries

Exception handling

Third-party libraries

Data formatting
