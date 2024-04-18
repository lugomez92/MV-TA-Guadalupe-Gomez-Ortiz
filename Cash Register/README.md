# Cash Register Application

The Cash Register Application replicates the functionality of a physical cash register. It enables easy addition and removal of items, counts coins and bills, calculates total amounts, and efficiently determines change for transactions. Ideal for retail and business environments, it streamlines cash management processes with accuracy and ease.

## Collaborators
- Anastasia Lukavsky
- Bridget Galang
- Mei Huang

## Functions

1. **removeItem(name, drawer)**:
   - This function decreases the quantity of a specific currency item in the cash drawer.
   - It takes the name of the currency item to be removed and the current state of the drawer as inputs.
   - After finding the currency item with the specified name in the drawer, it decrements its quantity by one.

2. **addItem(name, drawer)**:
   - This function increases the quantity of a specific currency item in the cash drawer.
   - Similar to `removeItem`, it takes the name of the currency item and the current drawer state as inputs.
   - Once it finds the currency item with the specified name, it increments its quantity by one.

3. **countCoins(drawer)**:
   - This function counts the total number of coins (currency with values less than $1) in the cash drawer.
   - It iterates over each currency item in the drawer and accumulates the quantities of coins.
   - The total count of coins is then returned.

4. **countNotes(drawer)**:
   - This function counts the total number of notes (currency with values equal to or greater than $1) in the cash drawer.
   - It iterates through each currency item in the drawer and adds up the quantities of notes.
   - The total count of notes is then returned.

5. **sumDrawer(drawer)**:
   - This function calculates the total value of the cash drawer in dollars.
   - It iterates over each currency item in the drawer, multiplies its value by its quantity, and accumulates the total.
   - The sum is returned as a string formatted as a dollar amount.

6. **canMakeAmount(target, drawer)**:
   - This function checks if it's possible to make a specific amount using the coins and notes in the cash drawer.
   - It recursively explores combinations of currency items to see if they can sum up to the target amount.
   - Returns `true` if the amount can be made, `false` otherwise.

7. **transaction(cost, paid, drawer)**:
   - This function simulates a transaction by calculating the change to be given based on the cost of an item and the amount paid by the customer.
   - It calculates the change by subtracting the cost from the amount paid and then selects the appropriate coins and notes from the drawer to give as change.
   - Finally, it updates the drawer by adding the paid amount and removing the change given.
   - The updated drawer state is returned after the transaction.
