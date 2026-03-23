# Find Exercise

Please download the following zip file, unzip it, and navigate to the `Cases/` directory.

[Cases.zip](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/06091973-41ef-4e9f-bcf8-e3f2701d43f3/Cases.zip)

**Note: in order for this exercise to work out, please avoid modifying any of the case files!**

## Your Task

Welcome detective! The `Cases` folder contains a couple thousands case files, both open and closed. Please use the `find` command to assist you in the following tasks:

1. Using `find` (and another command), count the number of case files that include "closed", in lowercase, in their name. You should find **980** cases.
2. Oh no, one of our new detectives labels his cases using "CLOSED" in all caps. Find the 3 cases that have "CLOSED" in their name.
3. Get a total count of all closed cases that include "closed" in their name, uppercase or lowercase. You should get a count of 983!
4. Get a count for the total number of **open** cases with odd numbered case numbers (find the open cases that have a 1,3,5,7, or 9 as the last digit in their case number). You should get 519 cases.
5. Find the three empty cases
6. Most of these files are quite small, but there are 3 pretty large case files. Find the three files that are larger than 20k in size
7. Find the one case file that is larger than 150k and is closed
8. No one has touched these case files in years, or at least no one should have touched these files, but sadly some corrupt detective recently tampered with one of the files. Sometime today he changed a single case from "closed" to "open" to spite an enemy of his. Find the one case that has been modified more recently than the `yesterday.txt` file. Watch the exercise intro video if you're confused! You may need to read the man pages to find the correct command.
