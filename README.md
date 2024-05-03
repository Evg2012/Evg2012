import random

def roll_dice():
    return random.randint(1, 6)

def main():
    print("Welcome to Dice Roll Game!")
    player1_name = input("Enter player 1's name: ")
    player2_name = input("Enter player 2's name: ")

    player1_score = 0
    player2_score = 0

    for i in range(5):
        input(f"\nRound {i+1}: Press Enter to roll dice for {player1_name}")
        player1_roll = roll_dice()
        print(f"{player1_name} rolled: {player1_roll}")
        player1_score += player1_roll

        input(f"Press Enter to roll dice for {player2_name}")
        player2_roll = roll_dice()
        print(f"{player2_name} rolled: {player2_roll}")
        player2_score += player2_roll

    print("\nFinal Scores:")
    print(f"{player1_name}: {player1_score}")
    print(f"{player2_name}: {player2_score}")

    if player1_score > player2_score:
        print(f"\n{player1_name} wins!")
    elif player2_score > player1_score:
        print(f"\n{player2_name} wins!")
    else:
        print("\nIt's a tie!")

if __name__ == "__main__":
    main()
- 👋 Hi, I’m @Evg2012
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Evg2012/Evg2012 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
