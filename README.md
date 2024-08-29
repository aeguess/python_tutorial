# python_tutorial

The main data types native to Python are:
```
Boolean (True / False)

String ("Hello", "AB", "arg", "yarg", "1", "24", etc.)

Integer (-20, -1, 0, 50, 100000, etc.)

Float (3.1415, 86.90, 1.0, -10.0, etc.)

List (Example: ['a', 1, '42', 'springFIELD', 'a1-43-24', 26.0] )

```
(NOTE: There's technically also a dict() datatype, which allows you to store key-value pairs, but I've personally found that the Pandas library has sufficient functions and the Pandas.DataFrame() object does everything you'd need from the native dict() type, and more). 

-> A Boolean is simply a True/False. This is useful for indexing through lists, or applying screening parameters, or executing an if/else statement. E.g., "if X is True, do Y". 

-> a string are anything in "quotes" (so for example, the word Hello would need to be passed as 'Hello' or "Hello.  You can also pass numbers, special characters, or combinations of these into Python. 'app1e pi3 is-my-fav0rite ## f@@d' is a valid string. Without quotes, Python would return an error. During the Camp Fire project, this was relevant because housing data was often in the form of "XX-1111", which was a combination of numbers (1111), letters (XX), and special characters (-). To separate whether an animal was outside, I had to cut off the "-1111" from the string, and exclusively obtain the "XX".

-> An integer is a number. The main difference between it and a float, which also stores a number, is that an integer uses significantly less storage space. If you wanted to iterate through a for-loop, e.g. "for i in range(5): ", i would return an integer for every pass. Generally, if the number does NOT need decimal places, use an integer.

-> A float is a more precise integer, at the cost of more storage space. Needed to store decimal place values (e.g. 34 versus 34.1234)

-> A list is a... collection of things. A list can be exclusively integers, floats, strings, booleans, or any combination of other data types. Generally though, it's easier to work with lists that have values all of the same data type. For example, you could perform an operation on a list:

```
my_list = [1, 2, 3, 4]
for number in my_list:
  number = number*number # squares the value

print(my_list) # returns [1, 4, 9, 16]
```

The structure of a function can be written like so:
```
def my_function():
    print("Hello world")

my_function()  # calls my_function, outputs "Hello world"
```

Or
```
def my_function(arg_1):
    print("Hello " + str(arg_1))

my_function() # calls my_function... but this errors!
my_function("Joe") # calls my_function, passing the string "Joe" as an input argument. 
```

