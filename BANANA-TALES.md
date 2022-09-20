# BANANA TALES: CHALLENGE 65 - WHILE LOOPS
````
for index in range(len(wells)):
    print("Index is:")
    print(index)
    print("Max water level is:")
    print(wells[index].max_water_level)
    print("Water level is:")
    print(wells[index].water_level)
    while wells[index].water_level < wells[index].max_water_level:
        elephants[index].spray_at(wells[index])
````

# BANANA TALES: CHALLENGE 64 - WHILE LOOPS
````
for index in range(len(wells)):
    while wells[index].water_level < wells[index].max_water_level:
        elephants[index].spray_at(wells[index])
````


# BANANA TALES: CHALLENGE 63 - WHILE LOOPS

````
while wells[1].water_level < wells[1].max_water_level:
    elephants[1].spray_at(wells[1])
while wells[0].water_level < wells[0].max_water_level:
    elephants[0].spray_at(wells[0])
````



# BANANA TALES: CHALLENGE 57 - IF ELSE
````
for obstacle in obstacles:
    if obstacle.is_ice():
        dragon.fire_at(obstacle)
    else:
        dragon.smash(obstacle)
````

# OR
````
for obstacle in obstacles:
    if obstacle.is_ice():
        dragon.fire_at(obstacle)
    if obstacle.is_fence():
        dragon.smash(obstacle)
````


# BANANA TALES: CHALLENGE 56 - IF ELSE
````
for obstacle in obstacles:
    if obstacle.is_ice():
        dragon.fire_at(obstacle)
    else:
        dragon.smash(obstacle)
````


# BANANA TALES: CHALLENGE 55 - IF ELSE
````
# Need to manually plant 3x crates in holes in road!
for obstacle in obstacles:
    if obstacle.is_ice():
        dragon.fire_at(obstacle)
    if obstacle.is_fence():
        dragon.smash(obstacle)
````

# BANANA TALES: CHALLENGE 54 - IF ELSE
````
for obstacle in obstacles:
    if obstacle.is_box():
        dragon.smash(obstacle)
````



# BANANA TALES: CHALLENGE 53 - IF ELSE

````
# Solution in 6 lines
# 0, 2, 4 
#  8, 10
# skip 6

for i in range(-1,11):
    if i == 6:
        # do nothing
    else:
        if obstacles[i].is_ice():
           dragon.fire_at(obstacles[i])
````

````
# Solution in 4 lines
# 0, 2, 4, 6, 8, 10 then destroy blocking block

for i in range(-1,11):
    if obstacles[i].is_ice():
        dragon.fire_at(obstacles[i])
dragon.smash(obstacles[7])

````
````
# Solution in 4 lines
# 0, 2, 4, 6, 8, 10 then destroy blocking block

for obstacle in obstacles:
    if obstacle.is_ice():
        dragon.fire_at(obstacle)
dragon.smash(obstacles[7])
````




# BANANA TALES: CHALLENGE 52 - IF ELSE
````
# nb need to build three crates manually before running code
for obstacle in obstacles:
    if obstacle.is_ice():
        dragon.fire_at(obstacle)
````

# BANANA TALES: CHALLENGE 51 - IF ELSE
````
for obstacle in obstacles:
    if obstacle.is_ice():
        dragon.fire_at(obstacle)
````

# BANANA TALES: CHALLENGE 50 - IF ELSE
````
for index in range(0,6):
    dragon.fire_at(obstacles[index])
````



# BANANA TALES: CHALLENGE 49 - IF ELSE
````
for index in range(0,4):
    dragon.smash(obstacles[index])
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

# BANANA TALES: CHALLENGE 45 - VARIABLES

````
goal_height = giraffes[0].height + 1

for index in range(len(giraffes)):
    goal_height = goal_height + 1
    giraffes[index].height = goal_height 

````


# BANANA-TALES-CHALLENGE 44 - VARIABLES

````
goal_height = giraffes[0].height

for index in range(len(giraffes)):
    giraffes[index].height = goal_height      
````



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





