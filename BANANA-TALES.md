# BANANA-TALES-CHALLENGE 40 - RANGE  
```
# Change the giraffes with indexes 4 to 11

# 4,5,6,7,8,9,10,11
for index in range(4,12):
    giraffes[index].height = 5
    
# Change the snakes with indexes 2 to 6
for index in range(2,7):
    snakes[index].length = 2
    # Set the snakes' lengths
```

# BANANA-TALES-CHALLENGE 44 - VARIABLES

```
goal_height = giraffes[0].height

for index in range(len(giraffes)):
    giraffes[index].height = goal_height      
````

# BANANA TALES: CHALLENGE 45 - VARIABLES

````
goal_height = giraffes[0].height + 1

for index in range(len(giraffes)):
    goal_height = goal_height + 1
    giraffes[index].height = goal_height 
````
# BANANA TALES: CHALLENGE 46 - VARIABLES

````
#height = 2

#for giraffe in giraffes:
    # set the height of each giraffe using
    # the variable height
    
    # increase the value of height by 2
    
goal_height = giraffes[0].height

for index in range(len(giraffes)):
    giraffes[index].height = goal_height 
    goal_height = goal_height + 2
````

# BANANA TALES: CHALLENGE 47 - VARIABLES
````
#height = 8

#The giraffes' height needs to decrease by 1 each time
    
goal_height = 8

for index in range(len(giraffes)):
    giraffes[index+1].height = goal_height 
    goal_height = goal_height - 1
````
