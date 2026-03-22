Online Voting System (Python)

Introduction to OVS This is a CLI based Online Voting System developed as a part of the Introduction to Problem Solving and Programming course. While the course dives into functional programming, data validation, and dictionary-based state management.

Project Logic

This system works with a flow to maintain the election integrity:

Authentication: Matches Voter ID with "Already Voted" list.

Choice: Users select from a changing pool of candidates.

To avoid unintentional duplicate entries and filter out invalid inputs, validation is necessary.


Finalization: Shows the winner and total tally

The Source Code

Online Voting System - Python Project
Course: Introduction to Problem Solving and Programming

def run_election():
    # Initial Data
    candidates = ["Alice", "Bob", "Charlie"]
    vote_counts = {candidate: 0 for candidate in candidates}
    voted_ids = set() # To track unique voters
    
    print("--- Welcome to the Online Voting System ---")
    
    while True:
        print("\nOptions: [1] Vote [2] See Results [3] Exit")
        choice = input("Select an option: ")

        if choice == '1':
            voter_id = input("Enter your unique Voter ID: ").strip()
            
            if voter_id in voted_ids:
                print("Error: This ID has already cast a vote.")
                continue
            
            print("\nCandidates:")
            for i, name in enumerate(candidates, 1):
                print(f"{i}. {name}")
            
            try:
                selection = int(input("Enter candidate number: "))
                if 1 <= selection <= len(candidates):
                    chosen_candidate = candidates[selection - 1]
                    vote_counts[chosen_candidate] += 1
                    voted_ids.add(voter_id)
                    print(f"Success! You voted for {chosen_candidate}.")
                else:
                    print("Invalid candidate selection.")
            except ValueError:
                print("Invalid input. Please enter a number.")

        elif choice == '2':
            print("\n--- Current Election Standings ---")
            for candidate, votes in vote_counts.items():
                print(f"{candidate}: {votes} votes")
            
            winner = max(vote_counts, key=vote_counts.get)
            if vote_counts[winner] > 0:
                print(f"\nLeading Candidate: {winner}")
            else:
                print("\nNo votes cast yet.")

        elif choice == '3':
            print("Exiting system. Final results saved.")
            break
        else:
            print("Invalid choice. Try again.")

if __name__ == "__main__":
    run_election()



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




