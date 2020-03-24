# Div-3-and-5
#This is a python project to create an app that lists numbers between 0 and 100 skipping those divisible by 3 and 5

import time
l1 = list(range(100))    # creates a list l1 with numbers 0 to 100
l2 = []
l3 = []
l4 = []
l5 = []
l6 = []
for n in range(100):
    if (n%3) != 0:  # checks if the numbers in l1 are not divisible by 3
        l2.append(n)  # adds the numbers not div by 3 to l2
        l3 = l2.copy() # copies the values in l2 to l3


        if (n%5) != 0: # checks if the numbers are not div by 5 also
            l4.append(n)
            lf = l4.copy()
            
        else:
            l5.append(n)


    else:
        l6.append(n)
    
print("Numbers between 0 and 100 not divisible by 3 and 5: \n",lf)
print("\n Numbers not divisible by 3 but div by 5: \n",l5)
print("\n Numbers divisible by 3: \n", l6)

time.sleep(60) # suspends compilation for 60 seconds
quit() # closes the terminal
