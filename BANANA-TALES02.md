# BANANA TALES02
Before starting these lessons watch:
[Everything you need to know about Classes in Python! (Object Oriented Programming Tutorial)](https://www.youtube.com/watch?v=tmY6FEF8f1o)


#BANANA TALES: CHALLENGE 92 - CLASSES
```
class Drill:
    def __init__(self, x, y):
        self.x = x
        self.y = y
    
    def drill_right(self, count):
        self.x = self.x + count
    
# Define FOUR instances of Drill.
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
