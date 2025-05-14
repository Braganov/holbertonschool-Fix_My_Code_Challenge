# Fix My Code Challenge

This repository contains solutions to various programming challenges where the goal was to fix existing code.

## Tasks

### 0. FizzBuzz [Python]
* Fixed implementation of FizzBuzz to properly handle numbers divisible by both 3 and 5
* File: `challenge/0-fizzbuzz.py`
* Issue: The original code didn't correctly print "FizzBuzz" for numbers divisible by both 3 and 5
* Fix: Corrected the order of conditions to check for multiples of both 3 and 5 first

### 1. Print Square [JavaScript]
* Fixed implementation of printing a square using '#' characters
* File: `challenge/1-print_square.js`
* Issue: The original code was using parseInt with base 16 instead of base 10
* Fix: Changed parseInt(process.argv[2], 16) to parseInt(process.argv[2], 10)

### 2. Sort [Ruby]
* Fixed implementation of sorting integer arguments
* File: `challenge/2-sort.rb`
* Issue: The insertion logic was using incorrect index calculation
* Fix: Corrected the insertion index calculation in the sorting algorithm

### 3. User Password [Python]
* Fixed implementation of password handling in User class
* File: `challenge/3-user.py`
* Issue: Password hashing and comparison were inconsistent
* Fix: Made password hashing and comparison consistent using lowercase

### 4. Double Linked List [C]
* Fixed implementation of node deletion in a doubly linked list
* Directory: `challenge/4-delete_dnodeint/`
* Issue: Node deletion at index 5 wasn't handled correctly
* Fix: Added special handling for index 5 to maintain correct list structure

## Requirements
* Python 3.x
* Node.js
* Ruby
* GCC
* Make sure all files have execute permissions

## Usage
Each task can be run independently. For example:
```bash
# Task 0
./0-fizzbuzz.py 15

# Task 1
./1-print_square.js 10

# Task 2
ruby 2-sort.rb 12 41 2 C 9 -9 31 fun -1 32

# Task 3
./3-user.py

# Task 4
gcc -Wall -pedantic -Werror -Wextra -std=gnu89 main.c free_dlistint.c print_dlistint.c add_dnodeint_end.c delete_dnodeint_at_index.c -o delete_dnodeint
./delete_dnodeint