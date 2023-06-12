
num_friends = int(input("Enter the number of friends joining (including you):\n"))

if num_friends <= 0:
    print("No one is joining for the party")
else:
    print("Enter the name of every friend (including you), each on a new line:")
    friends = {}
    for _ in range(num_friends):
        name = input()
        friends[name] = 0

    print(friends)
total_bill = float(input("Enter the total bill:"))
    split_value = round(total_bill / num_friends, 2)
    split_dictionary = {}

    for i in range(1, num_friends + 1):
        split_dictionary[f"Friend {i}"] = split_value

    print(split_dictionary)
