Comp218
Adarsh Kumar
Assignment 2
3787647
time spent: 3.5 to 4 hours
------------
1. 
Similarities:
- Both use hashing to ensure that looking up an item takes the same amount of time regardless of how large the collection is.
- Both are mutable.
- Empty sets are created useing set() since {} defaults into a empty dictionary

Differences:
- A set only cares if an item exists, while a dictionary associates the key with the value
- If duplicates are added to a set, it is ignored, but when added to a dictionary, it overwrites the old value associated with the key

You can use a set to remove duplicated and for other mathematical operations, while dictionaries can be used to store a user's profile, count frequency, and for configuration

2. 
def fibo(n):

    fl = []

    # Initialize an empty list to store the sequence

    # Check if input is not an integer or is negative and return the empty list if so

    if not isinstance(n, int) or n < 0:
        return fl 
    fl = [1, 1] 

    # Set the first two numbers

    # Loop from the 3rd element up to the n-th element

    for i in range(2, n+1):

        # Calculate the next number by adding the previous two and append to list

        fl += [fl[i-1] + fl[i-2]] 

    return fl 

    # Return the completed list


    3. 
    The script finds all the factors of the variable by checking if every integer higher than 1 up to number can divide into it without a remainder.

    Output:
    factors of 32 are [1, 2, 4, 8, 16]


    4. 
    def outer():
    greeting = 'Good morning!'
    
    # The inner function that closes over the outer variable
    def greet(who):
        # Uses the greeting variable from the outer function
        print(greeting, who)
        
    # Returns the inner function object
    return greet

# 'cl' now holds the greet function
cl = outer()

# Executes the inner function
cl('Joe')

Output: Good morning! Joe


