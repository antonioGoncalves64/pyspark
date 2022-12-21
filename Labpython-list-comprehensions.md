# python

## List Comprehensions and Generators



<a target="_blank" href="https://colab.research.google.com/github/antonioGoncalves64/pyspark/blob/main/Labpython-list-comprehensions.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

List Comprehensions is an elegant way of defining and creating a list. List Comprehension allows us to create a list using for loop with lesser code. What normally takes 3-4 lines of code, can be compressed into just a single line. Example:

    list_comprehension = [i for i in range(11) if i % 2 == 0]
 
Generator Expressions are somewhat similar to list comprehensions, but the former doesn’t construct list object. Instead of creating a list and keeping the whole sequence in the memory, the generator generates the next element in demand.
When a normal function with a return statement is called, it terminates whenever it gets a return statement. But a function with a yield statement saves the state of the function and can be picked up from the same state, next time the function is called.
The Generator Expression allows us to create a generator without the yield keyword. Example:

    generator_expression = (i for i in range(11) if i % 2 == 0)
    
    
Difference between Generator Expressions and List Comprehensions. The generator yields one item at a time and generates item only when in demand. Whereas, in a list comprehension, Python reserves memory for the whole list. Thus we can say that the generator expressions are memory efficient than the lists.

We can say that generator Expressions are a special kind of function that return a lazy iterator. These are objects that you can loop over like a list. However, unlike lists, lazy iterators do not store their contents in memory.
