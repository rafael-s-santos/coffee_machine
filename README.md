<h2 align="center">Coffee Machine</h2>

<p align="center"><img src="\resources\banner.png" height="320" /></p>

EN | [PT](https://github.com/rafael-s-santos/coffee_machine/blob/main/resources/README_PT_BR.md)

<p align="center">Putting Object-Oriented Programming Concepts into Practice</p>

This is a Python program for a coffee machine that allows users to select and purchase various coffee beverages. The program has the following features:

## Requirements

1. ### Prompt the user by asking "What would you like? (espresso/latte/cappuccino):"
   - Check the user input to decide what to do next.
   - The prompt should appear every time an action is completed, e.g., when the drink is dispensed. The prompt should reappear to serve the next customer.

2. ### Turn off the coffee machine by typing "off" at the prompt.
   - The coffee machine maintainers can use "off" as a secret word to turn off the machine. Your code should terminate when this happens.

3. ### Print a report.
   - When the user enters "report" at the prompt, a report should be generated showing the current resource values, e.g.,
     ```
     Water: 100ml
     Milk: 50ml
     Coffee: 76g
     Money: $2.5
     ```

4. ### Check if there are sufficient resources?
   - When the user chooses a drink, the program should check if there are enough resources to make that drink.
   - For example, if Latte needs 200ml of water but there is only 100ml left in the machine, it should not continue to prepare the drink but print: "Sorry, there is not enough water."
   - The same should happen if another resource runs out, e.g., milk or coffee.

5. ### Process coins.
   - If there are sufficient resources to select the drink, the program should ask the user to insert coins.
   - Remember that quarters = $0.25, dimes = $0.10, nickels = $0.05, pennies = $0.01.
   - Calculate the monetary value of the coins inserted. For example, 1 quarter, 2 dimes, 1 nickel, 2 pennies = $0.52.

6. ### Check if the transaction was successful?
   - Check if the user inserted enough money to buy the selected drink. For example, the latte costs $2.50, but they inserted only $0.52, and after counting the coins, the program should say "Sorry, not enough money. Money refunded."
   - But if the user inserted enough money, the cost of the drink will be added to the machine as profit, and this will be reflected the next time the "report" is triggered. For example:
   
     ```
     Water: 100ml
     Milk: 50ml
     Coffee: 76g
     Money: $2.5
     ```

   - If the user has inserted too much money, the machine should offer change. For example, "Here is $2.45 in change." The change should be rounded to 2 decimal places.

7. ### Make coffee.
   - If the transaction is successful, and there are enough resources to prepare the drink selected by the user, the ingredients to make the drink should be deducted from the coffee machine's resources.
   - For example, inform before buying a latte:

     ```
     Water: 300ml
     Milk: 200ml
     Coffee: 100g
     Money: $0
     ```

   - Report after buying a latte:

     ```
     Water: 100ml
     Milk: 50ml
     Coffee: 76g
     Money: $2.5
     ```

   - After all resources are deducted, tell the user "Here is your latte. Enjoy!" if a latte was their chosen beverage.

## Getting Started
To run the Coffee Machine Program, follow these steps:

1. Make sure you have Python installed on your computer.
2. Clone this repository to your local machine.
3. Open your terminal or command prompt and navigate to the directory where you cloned the repository.
4. Run the `coffee_machine.py` script by executing the following command:
```
python coffee_machine.py
```
5. Follow the on-screen instructions to interact with the coffee machine.

Enjoy your coffee! ☕
