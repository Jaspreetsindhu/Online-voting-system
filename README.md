Online Voting System (Python)

Introduction to OVS This is a CLI based Online Voting System developed as a part of the Introduction to Problem Solving and Programming course. While the course dives into functional programming, data validation, and dictionary-based state management.

Project Logic

This system works with a flow to maintain the election integrity:

Authentication: Matches Voter ID with "Already Voted" list.

Choice: Users select from a changing pool of candidates.

To avoid unintentional duplicate entries and filter out invalid inputs, validation is necessary.


Finalization: Shows the winner and total tally

The Source Code



File
## How to Run

To start you need to clone the repository.

Here is how you can do it:

Bash

git clone https://github.com/yourusername/online-voting-python.git

Next navigate to the directory.

Just use this command:

Bash

cd online-voting-python

Now you can execute the script.

Here is the command:

Bash

python voting_system.py

## Key Concepts Applied

The code uses key concepts.

One of them is Sets.

Sets are used for voted_ids.

This is done to ensure fast lookup time, O(1). To prevent people from voting twice.

Another concept used is Dictionaries.

Dictionaries are used for vote_counts.

They map candidates to their votes.

The code also handles errors.

It uses try-except blocks.

These blocks manage inputs that're not integers.

Loops are also used.

A while True loop is used.

This loop keeps the voting station active until it is manually closed.




