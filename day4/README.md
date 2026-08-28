# Day 4 - Text Processing

## Objective

To practice Linux text-processing commands and pipelines.

## Commands Practiced

- grep
- awk
- sed
- sort
- uniq
- cut
- tr
- wc
- Pipelines

## Practice File

students.txt

Format:

Name,Department,Mark

## grep

Used to search for matching text.

Example:

grep "AI" students.txt

Result:
4 AI students found.

## awk

Used to extract fields and perform calculations.

$1 = Name
$2 = Department
$3 = Mark

Marks above 80:

Arun 85
Charan 91
Gokul 88
Kiran 95
Ravi 82

AI students above 80:

Charan 91
Arun 85
Ravi 82

Average mark:

80

## sed

Used for text substitution, printing selected lines, and deleting lines.

Examples:

sed 's/AI/AIDS/g' students.txt
sed -n '1,5p' students.txt
sed '4d' students.txt

## sort

Used to sort data.

Numeric ascending:
64 68 72 76 79 82 85 88 91 95

Numeric descending:
95 91 88 85 82 79 76 72 68 64

Students were also sorted by marks in descending order.

## uniq

Used to remove duplicate consecutive values and count occurrences.

Department counts:

AI = 4
CSE = 3
ECE = 3

## cut

Used to extract fields.

-f1 = Name
-f2 = Department
-f3 = Mark

## tr

Used to translate or delete characters.

Examples:

Lowercase to uppercase
Uppercase to lowercase
Comma to space
Delete digits

## wc

Used to count lines, words and characters.

students.txt:

Lines = 10
Words = 10
Characters = 123

AI student count = 4

## Pipelines

Commands were combined using the pipe symbol `|`.

Examples:

grep "AI" students.txt | cut -d',' -f1

cut -d',' -f2 students.txt | sort | uniq -c

sort -t',' -k3,3nr students.txt | head -3

## Status

Day 4 - Text Processing completed successfully.
