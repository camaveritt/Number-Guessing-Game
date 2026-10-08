# Number Guessing Game

A command-line number guessing game written in Bash, with a PostgreSQL database to track players and their scores.

The game picks a random number between 1 and 1000 and gives higher/lower hints until you guess it. It remembers each player's number of games played and best score.

## Setup

1. Create the database and tables:

   ```bash
   psql -U postgres -f number_guess.sql
   ```

2. Run the game:

   ```bash
   chmod +x number_guess.sh
   ./number_guess.sh
   ```

## Example

```
Enter your username:
alex
Welcome, alex! It looks like this is your first time here.
Guess the secret number between 1 and 1000:
500
It's higher than that, guess again:
750
It's lower than that, guess again:
620
You guessed it in 3 tries. The secret number was 620. Nice job!
```

## Built With

- Bash
- PostgreSQL
