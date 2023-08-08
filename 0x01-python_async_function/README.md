# 0x01. Python - Async

### Asynchronous routines are able to “pause” while waiting on their ultimate result and let other routines run in the meantime. Asynchronous code, through the mechanism above, facilitates concurrent execution. To put it differently, asynchronous code gives the look and feel of concurrency

![ASYNC](https://user-images.githubusercontent.com/110098940/252291925-3ce833cb-0723-4650-ae3c-7d933663cb34.png)

# Executing an Async Program with asyncio  
- To execute an async program, you need to use the asyncio module, which provides an event loop to manage the execution of coroutines. Here's an example:

`
import asyncio  
 
async def my_coroutine():  
    # Async code goes here  

# Create an event loop  
loop = asyncio.get_event_loop()  

# Run the coroutine  
loop.run_until_complete(my_coroutine())  
`

# Running Concurrent Coroutines  
`asyncio` allows you to run multiple coroutines concurrently using the `asyncio.gather()` function. Here's an example:

`
import asyncio  

async def coroutine1():  
    # Coroutine 1 code  

async def coroutine2():  
    # Coroutine 2 code  

# Create an event loop  
loop = asyncio.get_event_loop()  

# Run multiple coroutines concurrently  
loop.run_until_complete(asyncio.gather(  
    coroutine1(),  
    coroutine2()  
))  
`

# Using the random Module
The `random` module provides functions for generating random numbers and making random choices. Here's an example of using the `random` module:  

`
import random  

# Generate a random integer between 1 and 10  
random_number = random.randint(1, 10)  

# Choose a random element from a list  
random_element = random.choice(['apple', 'banana', 'orange'])  
`

These are just basic examples, and the `random` module offers many more functions for various random operations.
