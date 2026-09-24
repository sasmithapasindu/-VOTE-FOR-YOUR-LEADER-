
Leaders = ["Saman", "Kamal", "Supun", "Amal"]

votes = [0, 0, 0, 0]

print("=== VOTE FOR YOUR LEADER ===")
for i in range(len(Leaders)):
    print(f"[{i + 1}] {Leaders[i]}")


vote = int(input("\nEnter The Number Of The Leader To Vote: "))
selected_index = vote - 1

if 0 <= selected_index < len(Leaders):
    votes[selected_index] = votes[selected_index] + 1
    print(f"Success! You voted for {Leaders[selected_index]}.")
else:
    print("Invalid choice! Please select a valid number to vote.")

while True:
    print ("\nDo you want to vote again? (yes/no)")
    choice = input()
    if choice == "no":
        break
    elif choice == "yes":
        print("=== VOTE FOR YOUR LEADER ===")
        for i in range(len(Leaders)):
            print(f"[{i + 1}] {Leaders[i]}")
        vote = int(input("\nEnter The Number Of The Leader To Vote: "))
        selected_index = vote - 1
        if 0 <= selected_index < len(Leaders):
            votes[selected_index] = votes[selected_index] + 1
            print(f"Success! You voted for {Leaders[selected_index]}.")
        else:
            print("Invalid choice! Please select a valid number to vote.")
    else:
        print("Invalid choice! Please enter 'yes' or 'no'.")

print("\n=== VOTE RESULTS ===")

for i in range(len(Leaders)):
    print(f"{Leaders[i]}: {votes[i]} vote(s)")

max_votes = max(votes)

if max_votes == 0:
    print("No votes were cast.")
else:
    winners = [Leaders[i] for i in range(len(Leaders)) if votes[i] == max_votes]
    if len(winners) == 1:
        print(f"The winner is {winners[0]} with {max_votes} vote(s)!")
    else:
        print(f"It's a tie between: {', '.join(winners)} with {max_votes} vote(s) each!")


from matplotlib import pyplot as plt


plt.title("Vote Results")

plt.bar(Leaders, votes, color=['blue', 'black', 'green', 'maroon'])
plt.xlabel("Leaders")
plt.ylabel("Number Of Votes")

plt.show()

