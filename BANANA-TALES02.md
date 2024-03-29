# BANANA TALES02
Before starting these lessons watch:
[Everything you need to know about Classes in Python! (Object Oriented Programming Tutorial)](https://www.youtube.com/watch?v=tmY6FEF8f1o)

[Banana Tales Part 2 - Python - Coding Concepts](https://help.codemonkey.com/en/articles/5177159-banana-tales-part-2-python-coding-concepts#h_0d3ab1b318)

#BANANA TALES: CHALLENGE 131 - 2D LISTS
```
clouds[1][0] = None
clouds[1][2] = None
clouds[2][0] = Cloud()
```

#BANANA TALES: CHALLENGE 130 - 2D LISTS
```
clouds[0][1] = Cloud()
clouds[0][5] = Cloud()
clouds[0][6] = Cloud()
```

# BANANA TALES CHALLENGE 128 -TUPLE
```
colors = ("green","blue","red","gold","white","gray")
for color in basket_1.balloon_colors:
    if color not in colors:basket_1.balloon_colors.remove(color)
for color in basket_2.balloon_colors:
    if color not in colors:basket_2.balloon_colors.remove(color)
for color in colors:basket_3.balloon_colors.add(color)
for color in colors:basket_4.balloon_colors.add(color)
```

# BANANA TALES CHALLENGE 127 -TUPLE
```
basic_colors = ("green", "blue", "red", "yellow")

for color in basket_1.balloon_colors:
    if color not in basic_colors:
        basket_1.balloon_colors.remove(color)
        
# Remove the colors that are not in basic_colors
# from basket_2
for color in basket_2.balloon_colors:
    if color not in basic_colors:
        basket_2.balloon_colors.remove(color)
```


# BANANA TALES CHALLENGE 126 -TUPLE
```
new_colors = ("white", "black", "pink", "purple", "orange")
for index in range(-1,5):
    for color in new_colors:
        print(color)
        baskets[index].balloon_colors.add(color)
```

# BANANA TALES CHALLENGE 125 -TUPLE
```
new_colors = ("red", "blue", "green", "purple", "yellow")

for color in new_colors:
    print(color)
    baskets[0].balloon_colors.add(color)
for color in new_colors:
    print(color)
    baskets[1].balloon_colors.add(color)
```

# BANANA TALES CHALLENGE 124 -TUPLE
```
new_colors = ("blue", "yellow", "brown", "red", "white", "green", "gray")

for color in new_colors:
    print(color)
    basket_1.balloon_colors.add(color) 
```

# BANANA TALES CHALLENGE 123 -SET
```
for index in range(0,4):
    color = baskets[0].balloon_colors.pop()
    print(color)
    baskets[1].balloon_colors.add(color)
```



# BANANA TALES CHALLENGE 122 -SET
```
for basket in baskets:
    basket.balloon_colors.pop()
    basket.balloon_colors.pop()
```



# BANANA TALES CHALLENGE 121 - SET

```
for basket in baskets:
    basket.balloon_colors.add("green")
    basket.balloon_colors.add("yellow")

```

# BANANA TALES CHALLENGE 120 - SET

```
baskets[1].balloon_colors.add("yellow")
for index in range(-1,4):
    baskets[index].balloon_colors.add("green")
    baskets[index].balloon_colors.add("red")
baskets[0].balloon_colors.pop()
```




# BANANA TALES CHALLENGE 119 - SET

```
# Note the following line of code exists in the setup.py: basket = Basket(11, 10, ["red"]) which explains why there are actually three different coloured balloons

basket.balloon_colors.add("yellow")

# Add another colored balloon to lift the basket.
basket.balloon_colors.add("green")
```


# BANANA TALES CHALLENGE 118 - SET

```
# The balloon_colors is a set. 
# Each color can appear in it only once.

basket.balloon_colors.add("blue")

basket.balloon_colors.add("yellow")

# Change it to a green balloon, to be added to the basket.
basket.balloon_colors.add("green")
```

# BANANA TALES CHALLENGE 117 - DICTIONARY

```
codes_and_passwords = rat.get_passwords()
for gate in gates:
    if gate.code in codes_and_passwords:
        password = codes_and_passwords[gate.code]
    if gate.code not in codes_and_passwords:
        password = 'zz' + gate.code
    gate.open(password)
```

# BANANA TALES CHALLENGE 116 - DICTIONARY

```
#three star - six lines or less of code
```

```
#two star
codes_and_passwords = rat.get_passwords()
# This code adds the missing password to the dictionary.
password = 'a' + gates[7].code + 'z'
codes_and_passwords[gates[7].code] = password
for gate in gates:
    if gate.code in codes_and_passwords:
        password = codes_and_passwords[gate.code]
        gate.open(password)
```

# BANANA TALES CHALLENGE 115 - DICTIONARY

```
#code exactly the same as previous solution
#there are simply more gates!
codes_and_passwords = rat.get_passwords()
print(codes_and_passwords)
for gate in gates:
    if gate.code in codes_and_passwords:
        password = codes_and_passwords[gate.code]
        gate.open(password)
```


# BANANA TALES CHALLENGE 114 - DICTIONARY

```
codes_and_passwords = rat.get_passwords()
print(codes_and_passwords)
for gate in gates:
    if gate.code in codes_and_passwords:
        password = codes_and_passwords[gate.code]
        gate.open(password)
```


# BANANA TALES CHALLENGE 113 - DICTIONARY
```
#code exactly the same as previous solution
#there are simply more gates!
codes_and_passwords = rat.get_passwords()
print(codes_and_passwords)
for gate in gates:
    password = codes_and_passwords[gate.code]
    gate.open(password)
```


# BANANA TALES CHALLENGE 112 - DICTIONARY

```
#three star
codes_and_passwords = rat.get_passwords()
print(codes_and_passwords)
for gate in gates:
    password = codes_and_passwords[gate.code]
    gate.open(password)

```


```
#two star
codes_and_passwords = rat.get_passwords()
print(codes_and_passwords)
password = codes_and_passwords[gates[0].code]
# Open the first gate.
gates[0].open(password)

password = codes_and_passwords[gates[1].code]
# Open the second gate.
gates[1].open(password)
```


# BANANA TALES CHALLENGE 111 - DICTIONARY

Hints  
1.In the dictionary challenges, you cannot build the password based on the gate's code. The rat will help you!  
2.The function get_passwords() returns a dictionary of codes and passwords of the closed gates.  
3.A dictionary is a collection of keys and values. It is written with curly brackets {}.  eg. {'earth': 'tvupp'}
4.The function get_passwords() returns a dictionary, where the keys are the gates' codes; the values are the gates' passwords.  
5.To get the value of a specific key, use the key inside square brackets [].  
6.To get the password of gate_1, use: codes_and_passwords[gate_1.code].  
7.Use password to open gate_1.  

```
codes_and_passwords = rat.get_passwords()
print(codes_and_passwords)
password = codes_and_passwords[gate_1.code]
print(password)
gate_1.open(password)
```





# BANANA TALES CHALLENGE 110 - STRINGS


```
#three star solution - 5 lines or less of code

```

```
#two star solution
for gate in gates:
    code = gate.code
    r = len(code)
    password = ""
#reverse password + code[index] to code[index] + password get the word in reverse!
    for index in range(r): password = code[index] + password
    gate.open(password)
```



# BANANA TALES CHALLENGE 109 - STRINGS



```
#three star solution
for gate in gates:
    code = gate.code
    password = code[5]
    print(password)
    for index in range(5): password = password + code[index]
    gate.open(password)
```

```
#two star solution
code = gates[2].code
password = code[5]
print(password)
for index in range(5): password = password + code[index]
gates[2].open(password)
        
code = gates[3].code
password = code[5]
print(password)
for index in range(5): password = password + code[index]
gates[3].open(password)

code = gates[4].code
password = code[5]
print(password)
for index in range(5): password = password + code[index]
gates[4].open(password)
```


# BANANA TALES CHALLENGE 108 - STRINGS
```
#three star solution
for gate in gates:
   password = ""
   code = gate.code
   for index in range(1, len(code)): password = password + code[index]
   gate.open(password)
```


```
#two star solution
password = ""
code = gates[2].code
for index in range(1, len(code)): password = password + code[index]
gates[2].open(password)

password = ""
code = gates[3].code
for index in range(1, len(code)): password = password + code[index]
gates[3].open(password)

password = ""
code = gates[4].code
for index in range(1, len(code)): password = password + code[index]
gates[4].open(password)

password = ""
code = gates[5].code
for index in range(1, len(code)): password = password + code[index]
gates[5].open(password)
```

# BANANA TALES CHALLENGE 107 - STRINGS
```
password = ""
code = gates[2].code
for index in range(1, len(code)): password = password + code[index]
gates[2].open(password)
```

# BANANA TALES CHALLENGE 106 - STRINGS
```
#three star solution
password = ""
code = gate_3.code
for c in code: password = c + password
gate_3.open(password)
```

```
#two star solution
password = ""
code = gate_3.code
for c in code:
    password = c + password
gate_3.open(password)
```

# BANANA TALES CHALLENGE 105 - STRINGS

```
#two star solution
for index in range(-1,4):
    password = ""
    code = gates[index].code
    for c in code:
        password = password + c + c
        print(password)
    # Use password to open the gate.
    gates[index].open(password)
```


```
#one star solution
password = ""
code = gates[3].code
for c in code:
    password = password + c + c
    print(password)
# Use password to open the gate.
gates[3].open(password)

# Open the last gate.
password = ""
code = gates[4].code
for c in code:
    password = password + c + c
    print(password)
# Use password to open the gate.    
gates[4].open(password)
```



# BANANA TALES CHALLENGE 104 - STRINGS

```
#three star solution
# open gate[0] and gate[2]
# gate[1] and gate[3] are open already
for index in range(-1,4):
    password = "ab" + gates[index].code + "yz"
    gates[index].open(password)
```

```
#two star solution
#open gate[0] and gate[2]
#gate[1] and gate[3] are open already
password = "ab" + gates[0].code + "yz"
gates[0].open(password)

password = "ab" + gates[2].code + "yz"
gates[2].open(password)
```

# BANANA TALES CHALLENGE 103 - STRINGS


Hints    
1.The operator + concatenates (adds) two strings into one: "a" + "b" becomes "ab".  
2.All passwords are built out of the code, using the same pattern.  
3.Look at the open gates to find out how to build the closed gate password, from the code.  
4.In this challenge, the password is the gate's code + the string "abc".  
5.Change the string "aaa" to "abc".  
```
# Build the password for gate_2.
password = gate_2.code + "abc"
gate_2.open(password)
```

# BANANA TALES CHALLENGE 102 - STRINGS
```password = gate_3.code
print(password)

gate_3.open(password)
```


# BANANA TALES CHALLENGE 101 - INTEGERS
```
snake.length = 2

# Get the index of the giraffe and the desired height
for index in range(0,4):
    index = int(input("Enter the girffe's index: "))
    giraffes[index].height = int(input("Enter the giraffes's height: "))
```

# BANANA TALES CHALLENGE 100 - INTEGERS

#one star solution
```
#What is interesting is the way the snakes are named in this challenge.
#The snakes in the challenge are:
#snake, snakes[0], snakes[1], snakes[2], snakes[3]
#Why not just name them snakes[0], snake[1], snake[2], snake[3], snake[4]

#input "snake length" as follows to complete the puzzle
# >>> Enter the snake's length: 9
# >>> Enter the snake's length: 7
# >>> Enter the snake's length: 6
# >>> Enter the snake's length: 4

# set length of "snake"
snake.length = 2
# set length of "snake[0]", "snake[1]", "snake[2]", "snake[3]"
for snake in snakes:
    snake.length = int(input("Enter the snake's length: "))
```
#three star solution - use --> int(input("Enter input") only twice
```
# BANANA TALES CHALLENGE 100 - INTEGERS
# What is interesting is the way this challenge has been made.
# The snakes in the challenge are:
# snake, snakes[0], snakes[1], snakes[2], snakes[3]

snake.length = 1
for index in range(0,4):
    index = int(input("Enter the snake's index: "))
    snakes[index].length = int(input("Enter the snake's length: "))
```
# BANANA TALES CHALLENGE 99 - INTEGERS
```
# Any input entered is a string, even digits.
# int() converts it to a number.
# on run input the integer to match the giraffe height required to match the height that the pigeon drops 
snake.length = 2
for giraffe in giraffes:
    giraffe.height = int(input("Enter the giraffe's height: "))
```




# BANANA TALES: CHALLENGE 98 - INTEGERS

```
snake.length = 2
# Any input entered is a string, even digits.
# int() converts it to a number.
height = int(input("Enter the giraffes's height: "))

# Use height to change the giraffe's height

giraffe.height = height
```


# BANANA TALES: CHALLENGE 97 - INPUT

```
# if the pigeon lands on the ground you must input 'down' to be able to complete the puzzle
# if the pigeon lands on the middle platform you must input 'middle' to be able to complete the puzzle
# if the pigeon lands on the uppder platform you must input 'up' to be able to complete the puzzle

snake.length = 1

answer = input("Type 'up', 'down' or 'middle': ")

if answer == 'up':
    height = 8
elif answer == 'down':
    height = 2
else:
    height = 5

for giraffe in giraffes:
    giraffe.height = height
```


# BANANA TALES: CHALLENGE 96 - INPUT

```
# this puzzle requires 'down' be inputed to complete
# the pigeon takes off and lands randomly.  If the pigeon doesn't land on the ground then the puzzle will not complete
snake.length = 2

print("Type 'up' or 'down'")

# Check the input and set the height accordingly.
if input() == 'down':
    height = 3
else:
    height = 7

for giraffe in giraffes:
    giraffe.height = height
```

# BANANA TALES: CHALLENGE 95 - INPUT

```
# this puzzle requires 'down' be inputed to complete
# the pigeon takes off and lands randomly.  If the pigeon doesn't land on the ground then the puzzle will not complete
snake.length = 2

print("Type 'up' or 'down'")
answer = input()

if answer == 'up':
    height = 11
else:
    height = 4
    
giraffes[0].height = height
giraffes[1].height = height
```


# BANANA TALES: CHALLENGE 93 - CLASSES

```
class Drill:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def drill_right(self, count):
        self.x = self.x + count

drill_1 = Drill(1,13)
drill_2 = Drill(5,12)
drill_3 = Drill(9,11)
drill_4 = Drill(13,10)

# Define two more (total of four) instances of Drill.


# Drill instances placed into a list.
drills = [drill_1, drill_2, drill_3, drill_4]

# Use a for loop.
for index in drills:
    index.drill_right(4)
```


# BANANA TALES: CHALLENGE 92 - CLASSES
```
class Drill:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def drill_right(self, count):
        self.x = self.x + count
    
# Define two more (total of four) instances of Drill.
drill_1 = Drill(2, 10)
drill_2 = Drill(2, 11)
drill_3 = Drill(10,12)
drill_4 = Drill(10,13)




# Count how many brick walls each drill needs to drill.
drill_1.drill_right(4)
drill_2.drill_right(7)
drill_3.drill_right(3)
drill_4.drill_right(5)
```





````
class Drill:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    def drill_right(self):
        self.x = self.x + 2

# Define instances of Drill, each with the correct x & y.
drill_1 = Drill(3,10)
drill_2 = Drill(5,8)
drill_3 = Drill(7,12)
drill_4 = Drill(7,13)


# Drill through the brick walls.
drill_1.drill_right()
drill_2.drill_right()
for index in range(3):
    drill_3.drill_right()
    drill_4.drill_right()
````



# BANANA TALES: CHALLENGE 90 - CLASSES
````
class Drill:
    def __init__(self):
        self.x = 6
        self.y = 12
    
    def drill_right(self):
        self.x = self.x + 2

drill_1 = Drill()

# Drill through three bricks.

for index in range(3):
    drill_1.drill_right()
````

# BANANA TALES: CHALLENGE 89 - CLASSES
````
class Drill:
    def __init__(self):
        self.x = 2
        self.y = 13
    
    def drill_right(self):
        self.x = self.x + 2

drill_1 = Drill()

# Drill a brick.
drill_1.drill_right()

# Drill another brick.
drill_1.drill_right()
````

# BANANA TALES: CHALLENGE 88 - CLASSES
````
class Drill:
    def __init__(self):
        self.x = 9
        self.y = 13
    
    def drill_right(self):
        self.x = self.x + 2

drill_1 = Drill()
drill_1.drill_right()
````
