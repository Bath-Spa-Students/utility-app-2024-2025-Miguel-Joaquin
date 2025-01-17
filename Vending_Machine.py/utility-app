# Vending Machine

print(""" ██▒   █▓▓█████  ███▄    █ ▓█████▄  ██▓ ███▄    █   ▄████     ███▄ ▄███▓ ▄▄▄       ▄████▄   ██░ ██  ██▓ ███▄    █ ▓█████ 
▓██░   █▒▓█   ▀  ██ ▀█   █ ▒██▀ ██▌▓██▒ ██ ▀█   █  ██▒ ▀█▒   ▓██▒▀█▀ ██▒▒████▄    ▒██▀ ▀█  ▓██░ ██▒▓██▒ ██ ▀█   █ ▓█   ▀ 
 ▓██  █▒░▒███   ▓██  ▀█ ██▒░██   █▌▒██▒▓██  ▀█ ██▒▒██░▄▄▄░   ▓██    ▓██░▒██  ▀█▄  ▒▓█    ▄ ▒██▀▀██░▒██▒▓██  ▀█ ██▒▒███   
  ▒██ █░░▒▓█  ▄ ▓██▒  ▐▌██▒░▓█▄   ▌░██░▓██▒  ▐▌██▒░▓█  ██▓   ▒██    ▒██ ░██▄▄▄▄██ ▒▓▓▄ ▄██▒░▓█ ░██ ░██░▓██▒  ▐▌██▒▒▓█  ▄ 
   ▒▀█░  ░▒████▒▒██░   ▓██░░▒████▓ ░██░▒██░   ▓██░░▒▓███▀▒   ▒██▒   ░██▒ ▓█   ▓██▒▒ ▓███▀ ░░▓█▒░██▓░██░▒██░   ▓██░░▒████▒
   ░ ▐░  ░░ ▒░ ░░ ▒░   ▒ ▒  ▒▒▓  ▒ ░▓  ░ ▒░   ▒ ▒  ░▒   ▒    ░ ▒░   ░  ░ ▒▒   ▓▒█░░ ░▒ ▒  ░ ▒ ░░▒░▒░▓  ░ ▒░   ▒ ▒ ░░ ▒░ ░
   ░ ░░   ░ ░  ░░ ░░   ░ ▒░ ░ ▒  ▒  ▒ ░░ ░░   ░ ▒░  ░   ░    ░  ░      ░  ▒   ▒▒ ░  ░  ▒    ▒ ░▒░ ░ ▒ ░░ ░░   ░ ▒░ ░ ░  ░
     ░░     ░      ░   ░ ░  ░ ░  ░  ▒ ░   ░   ░ ░ ░ ░   ░    ░      ░     ░   ▒   ░         ░  ░░ ░ ▒ ░   ░   ░ ░    ░   
      ░ 
""")
# Vending Machine
print(""" ──────────────────────────────DRINKS───────────────────────────────
      
 | Chocolate Milk                A1                     3.00       |
 | Energy Drink                  A2                     6.25       |
 | Ginger Ale                    A3                     4.75       |
 | Kool Aid                      A4                     10.50      |
 | Milo                          A5                     2.50       |
 | Water                         A6                     1.25       |
      
 ──────────────────────────────SNACKS───────────────────────────────
      
 | Brownie                       B1                     4.25       |
 | Chip                          B2                     3.00       |
 | Macaron                       B3                     10.50      |
 | Oreo                          B4                     2.75       |
 | Pocky                         B5                     8.50       |
 | Popcorn                       B6                     1.00       |
      
 ───────────────────────────────────────────────────────────────────""")
 
List = {
    "A1": {'name': 'Chocolate Drink', 'price': 3.00, 'quantity': 5}, 
    "A2": {'name': 'Energy Drink', 'price': 6.25, 'quantity': 3},
    "A3": {'name': 'Ginger Ale', 'price': 4.75, 'quantity': 1},
    "A4": {'name': 'Kool Aid', 'price': 10.50, 'quantity': 10},
    "A5": {'name': 'Milo', 'price': 2.50, 'quantity': 8},
    "A6": {'name': 'Water', 'price': 1.25, 'quantity': 4},

    "B1": {'name': 'Brownie', 'price': 4.2, 'quantity': 2},
    "B2": {'name': 'Chip', 'price': 3.00, 'quantity': 6},
    "B3": {'name': 'Macaron', 'price': 10.50, 'quantity': 0},
    "B4": {'name': 'Oreo', 'price': 2.75, 'quantity': 5},
    "B5": {'name': 'Pocky', 'price': 8.50, 'quantity': 3},
    "B6": {'name': 'Popcorn', 'price': 1.00, 'quantity': 9},
}

print("Welcome To Miguel Vending Machine.")
Purchase_History = []

# Function to display purchase history
def View_Purchase_History():
    if Purchase_History:
        print("\nYour purchase history:")
        for purchase in Purchase_History:
            print(f"- {purchase['name']} for {purchase['price']:2f}")
    else:
        print("You havent made any purchase yet.")
      
# Main loop to keep asking for item selection
while True:
    Item_Stuff = input ("Select an item (e.g., A1, A2, B1, B2, ect.) or type 'history' to see your purchase history or 'exit' to leave: ").upper()

    if Item_Stuff == 'EXIT':
        print("Thank you for using Miguel Vending Machine!")
        break # Exit the loop and end the program
    
    # View purchase history
    elif Item_Stuff == 'HISTORY':
        View_Purchase_History()

    # Confirm item if it is in the list
    elif Item_Stuff in List:
        Selected_Item = List[Item_Stuff]
        Stock = Selected_Item ['quantity']

        if Stock > 0: 
           print("====================================")
           print(f"You have selected {Selected_Item['name']} with {Stock} in stock.")
           print(f"Price {Selected_Item['price']:.2f}")
           print("====================================")
           Amount = Selected_Item['price']

           # Money Payment Loop
           while Amount > 0:
               Payment = float(input(f"Please insert an amount ${Amount:.2f}: "))
               if Payment >= Amount:
                   Change = Payment - Amount
                   print("====================================")
                   print(f"You have purchased {Selected_Item['name']}!")
                   print(f"Your change is {Change:.2f}")
                   print("====================================")
                   # Stock Update
                   Selected_Item['quantity'] -= 1
                   Purchase_History.append({'name': Selected_Item['name'], 'price': Selected_Item['price']})
                   break
               else:
                   print("Insufficient payment. Please insert more.")
                   Amount -= Payment

           # After a successful purchase, ask if the user wants to buy the same item again
           while True:
               Next_Purchase = input(f"Would you like to buy another {Selected_Item['name']}? (yes/no): ").lower()
               if Next_Purchase == "yes":
                  if Selected_Item['quantity'] > 0:
                      break # allow the user to proceed to buy again
                  else:
                      print(f"Sorry, {Selected_Item['name']} is out of stock.")
                      break # Exit Inner Loop if out of stock
               elif Next_Purchase == "no":
                   break # Exit the inner loop and allow the user to buy a new item
               else:
                  print("Please answer with 'yes' or 'no'.")

        else:
           print(f"Sorry, {Selected_Item['name']} is out of stock.")

    else:
        print("That's not in my shop. Please enter item selection.")
