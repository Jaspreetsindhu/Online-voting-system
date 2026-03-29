## Online Voting System (Python)

# Project Overview

This project is an online voting system. It was made using Python for a class on problem solving and programming. This system is like an election where people can vote see the results and make sure each voter only votes once with a special ID.

# Problem Statement

Traditional voting systems take a lot of time can have errors and are not transparent. We need a system that's simple works well and is secure. It should allow:

•	Easy voting

•	No one can vote than once

•	See results in real-time

# Proposed Solution

The solution is a voting system on the command line made in Python. It:

•	Lets users vote with an ID

•	Stores votes safely while its running

•	Shows current election standings

•	Stops people from voting more than once

# Features

•	🧑‍🤝‍🧑 Support for many candidates

•	🔐 Checks for a unique voter ID

•	📊 Counts votes in real-time

•	🚫 Stops duplicate voting

•	📈 Shows the leading candidate

•	🖥️ A interactive menu

# Technology Used

•	Programming Language: Python

•	Concepts Used:

•	Functions

•	Loops (while loop)

•	If-else statements

•	Dictionaries and Sets

•	Handling exceptions

# Working Principle

1.	The system starts with a list of candidates and their vote counts.

2.	Users choose from the menu:

•	Vote

•	View results

•	Exit

3.	When voting:

•	User enters their special voter ID

•	System checks if the ID has already voted

•	If not it records the vote

4.	Results update and show when asked.

# Project Structure

online-voting-system/
│
├── main.py        # Main Python script
├── README.md      # Project documentation


# Dataset Description

This project does not use any dataset.

Instead it uses:

•	A list of candidates that is already known (["Alice" "Bob" "Charlie"])

•	Data structures that are stored in the computers memory:

•	A dictionary to keep track of how votes each person gets

•	A set to keep track of who has already voted using their voter IDs


# How to Run the Project

1. First you need to get Python on your computer if you do not already have it.

2. Next you need to clone the project repository:

   git clone <(https://github.com/Jaspreetsindhu/Online-voting-system)>

3.	Navigate to the project folder:

    cd online-voting-system

4.	Run the program:

   python main.py


# Sample Interaction

--- Welcome to the Online Voting System ---

Options: [1] Vote [2] See Results [3] Exit
Select an option: 1

Enter your unique Voter ID: 123

Candidates:
1. Alice
2. Bob
3. Charlie

Enter candidate number: 2
Success! You voted for Bob.

Options: [1] Vote [2] See Results [3] Exit
Select an option: 2

--- Current Election Standings ---
Alice: 0 votes
Bob: 1 votes
Charlie: 0 votes

Leading Candidate: Bob

# Challenges Faced

•	We had to stop people from voting more than once. We used data structures to do this.

•	We had to deal with users entering data like words instead of numbers.

•	We wanted to make the command-line interface easy to use.

•	We had to update the system in time without using a database.

# Future Enhancements

•	We want to add a graphical user interface using tools like Tkinter or PyQt.

•	We plan to store data in a database like SQLite or MySQL.

•	A login system for users would be an addition.

•	We should add encryption to make voting secure.

•	Enabling access via a web app is also a plan.

# Learning Outcomes

•	We learned how to solve problems with Python.

•	We worked with data structures like dictionaries and sets.

•	We built a real-world voting system.

•	We got better at handling user input and exceptions.

•	We designed a command-line interface.

# Conclusion

The Online Voting System project shows how programming can solve real-world problems. It gives a model for secure voting and helps learn Python programming.

# Author

Jaspreet Sindhu

Reg No: 25BOE10069

Course: Introduction, to Problem Solving and Programming

   

# Output screenshot
![image](https://github.com/user-attachments/assets/964a0cf5-7259-49d9-b815-7a318a821c9d)



