##### Rock-Paper-Scissor
- Very first things that I learnt into my Python Journey

---
Rock, paper, scissors 
---
```bash
import random 

def get_choices(): 

  player_choice = input("Enter a choice (rock, paper, scissors): ") 

  options = ["rock", "paper", "scissors"] 

  computer_choice = random.choice(options) 

  choices = {"player": player_choice, "computer": computer_choice} 

  return choices 
```
   
```bash
def check_win(player, computer): 

  print (f"You_chose {player}, computer_chose {computer}") 

  if player == computer: 

    return "It's a tie" 

  elif player == "rock": 

    if computer == "scissors": 

     return "Rock smashes scissors! You win!" 

    else: 

      return "Paper covers rock! You loose." 

  elif player == "paper": 

   if computer == "rock": 

    return "Paper covers rock! You win!" 

   else: 

     return "Scissors cuts paper! You loose." 

  elif player == "scissors": 

   if computer == "paper": 

    return "Scissors cuts papers! You win!" 

  else: 

    return "Rock smashes scissors! You loose." 

 ```
```bash

choices = get_choices() 

result = check_win(choices["player"], choices["computer"]) 

print(result) 
```
