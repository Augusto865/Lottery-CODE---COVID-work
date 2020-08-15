# Lottery-CODE---COVID-work
Lottery code

import random

Chosen_lottery_numbers = []
for i in range (0,7):
  number = random.randint(0,50)
  while number in Chosen_lottery_numbers:
    number = random.randint(0,50)
  Chosen_lottery_numbers.append(number)

user_numbers = []
while len(user_numbers) < 7:
  number = int(input("Enter a number between 1 and 50 :"))
  if (number in user_numbers or number>50 or number<1):
    print("The number is invalid")
  else:
    user_numbers.append(number)

    
print("The lottery numbers are..")
print(Chosen_lottery_numbers)

print("Your chosen numbers were")
print(user_numbers)

if Chosen_lottery_numbers == user_numbers:
  print("Wow incredible, you have ridiculous luck")
else:
  Chosen_lottery_numbers != user_numbers
  print("Geez, You have bad luck")
