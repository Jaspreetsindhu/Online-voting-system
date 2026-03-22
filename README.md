Online Voting System (Python)

Introduction to OVS This is a CLI based Online Voting System developed as a part of the Introduction to Problem Solving and Programming course. While the course dives into functional programming, data validation, and dictionary-based state management.

Project Logic

This system works with a flow to maintain the election integrity:

Authentication: Matches Voter ID with "Already Voted" list.

Choice: Users select from a changing pool of candidates.

To avoid unintentional duplicate entries and filter out invalid inputs, validation is necessary.


Finalization: Shows the winner and total tally

The Source Code

Save the following code as voting_system. py:

Python

Online Voting System in Python Project

Problem Solving and Programming Foundations

def run_election():

Initial Data

candidates = ["Alice", "Bob", "Charlie"]

vote_counts = {candidate: 0 for candidate in candidates}

def init(self): # Initialize variables for votingSystem.

print("--- Welcome to the Online Voting System ---")

while True:

print(“\nSelect: [1] Vote [2] Results [3] Exit”)

choice = input("Select
