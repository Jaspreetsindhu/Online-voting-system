# Online-voting-system
The Secure Digital Ballot is a simplified software application designed to digitize the electoral process. The system allows administrators to set up an election, register candidates, and enables authenticated voters to cast their ballots electronically. The goal is to replace manual paper counting with an automated system that ensures accuracy.
Project Statement: Digital Voting System (Python)
1. Project Identification
Project Name: SecureVote Python CLI

Developer: [Your Name]

Course: Introduction to Problem Solving and Programming

Platform: Python 3.x (Console-Based)

2. Problem Description
The current process of manual voting in small-scale organizations (e.g., student councils, club elections) is inefficient, prone to tallying errors, and lacks immediate verification. There is a need for a lightweight, digital solution that automates the collection and counting of ballots while ensuring the integrity of the election by preventing unauthorized or duplicate voting.

3. Project Objectives
The primary goal is to develop a robust Python application that simulates a real-world election environment. The system must solve the following "Problem Solving" challenges:

Identity Verification: Distinguishing between registered and unregistered voters.

Concurrency Control: Ensuring a "One Person, One Vote" policy is strictly enforced.

Data Integrity: Maintaining accurate counts for multiple candidates simultaneously.

Error Resilience: Handling "bad data" (non-numeric inputs or out-of-range choices) without the program crashing.

4. Functional Requirements
The application shall provide the following capabilities:

A. Voter Module

Login System: Users must enter a pre-defined Voter ID to access the ballot.

Ballot Interface: Display a numbered list of candidates dynamically.

Vote Casting: Allow users to select a candidate by entering a corresponding index number.

Confirmation: Provide a success message once the vote is recorded.

B. Security Logic

Duplicate Prevention: If an ID has already voted, the system must trigger an "Access Denied" message.

Input Validation: The system must validate that the vote is a valid integer within the candidate range.

C. Administrative Module

Session Termination: A specific "Admin Key" (e.g., 999 or a password) to close the polls.

Result Tabulation: Upon closing, the system must calculate the total votes and declare the winner based on the highest count.

5. Technical Specifications (Python)
The project will utilize the following programming constructs:

Dictionaries: To map Candidate Names to Vote Totals and Voter IDs to Status.

While Loops: To keep the voting station active for multiple consecutive users.

Conditional Logic: (if/elif/else) to handle the flow of authentication and voting.

Exception Handling: (try/except) to manage ValueError during integer conversion.

6. Constraints & Scope
Scope: This version is a local console-based simulation and does not require a web interface or a persistent SQL database.

Data Persistence: Data is stored in-memory during the session (Optionally: Saved to a .txt file upon exit).
