# Guess-the-number
Input number to guess what number come out from random program in range 1 to 50. if out of range will return error. if false there will be question to try again.
## Sample of output
```
from random import randint

a = input("Enter a number between 1 to 50: ")
if int(a) > 50 or int(a) < 1:
  print("Error, please input from 1 to 50.")
else:
  y = randint(1, 50)
  for x in a:
    x = int(x)
    if x == y:
      print("You guessed it right!")
    else:
      print("You guessed it wrong!")
      print("The number was", y)
      z = input("Try again?:(Y/N)")
      if z == "Y":
        a = input("Enter a number between 1 to 50: ")
      else: 
        break
```
