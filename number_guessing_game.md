# Number Guessing Game Flowchart

This flowchart represents the logic of a Number Guessing Game. The game follows these steps:

1. The program generates a random number between 1 and 100.
2. The user is prompted to guess the number.
3. The program checks if the guess is correct:
   - If the guess is correct, the user wins.
   - If the guess is too high, the program informs the user and prompts for another guess.
   - If the guess is too low, the program informs the user and prompts for another guess.
4. The process repeats until the user guesses the correct number.

```mermaid
flowchart TD
    A[Start] --> B[Generate Random Number]
    B --> C[Prompt User for Guess]
    C --> D{Is Guess Correct?}
    D -->|Yes| E[User Wins]
    D -->|No| F{Is Guess Too High?}
    F -->|Yes| G[Inform User: Guess is Too High]
    F -->|No| H[Inform User: Guess is Too Low]
    G --> C
    H --> C
    E --> I[End]
