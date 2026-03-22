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

choice = input("Enter your choice: ")

if choice == '1':

voter_id = input("Enter your unique Voter ID: ") strip()

if voter_id in voted_ids:

print("Error: You have already voted with this ID.")

continue

print("\nCandidates:")

for i, name in enumerate(candidates, start=1):

print(f"{i}. {name}")

try:

selection = int(input("Регион номер кандидата: "))

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





