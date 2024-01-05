# Python_Vending_Machine

## Implement class: Vending Machine according to the following requirements:



• can be instantiated using the constructor Vending Machine(num_items, item_price) wher num items denotes the number of items in the machine, and item_price denotes the required number of coins to buy a single item.



• has a method buy(req_items, money) that represents a buy request where req_items denotes the requested number of items, and money is the amount the customer puts into the machine. Depending on the state of the machine, one of the following happens

• If there are enough items in the machine to serve the request and the given money is sufficient to buy the requested number of items, the number of items in the machine is reduced by the requested number of items. The method returns an integer denotes the change given back after the purchase.

• If there are fewer items in the machine than the requested number, it raises a ValueError exception with the message "Not enough items in the machine".


• If there are enough items in the machine to serve the request but the given amount of money is less than their cost, it raises a ValueError exception with the message "Not enough coins".

The class implementation will be tested by a provided code stub and several input files. Each input file contains parameters to test the implementation. First, the provided code stub initializes an instance of the Vending Machine. Next, it performs the given operations on the Vending Machine instance. The result of their execution will be printed to the standard output by the provided code.

Constraints

There will be at most 100 operations to be performed

# Vending Machine Project

This project implements a simple Vending Machine in Python. The Vending Machine class allows users to instantiate a vending machine with a specified number of items and item price. It provides a method to handle buy requests, checking if there are enough items and sufficient funds.

## Getting Started

### Prerequisites
- Python 3.x




## Class: VendingMachine
### Constructor

vm = VendingMachine(num_items, item_price)

## Method: Buy
try:
    change = vm.buy(req_items, money)
    print(f"Purchase successful. Change: {change}")
except ValueError as e:
    print(f"Error: {e}")

### Example:
# Instantiate Vending Machine
vm = VendingMachine(num_items=50, item_price=5)

# Perform buy operations
try:
    change = vm.buy(req_items=3, money=20)
    print(f"Purchase successful. Change: {change}")
except ValueError as e:
    print(f"Error: {e}")
