# Magic-8-Ball

# This program is to answer any "Yes" or "No" question with different fortune each time it executes

import random

# define a variable call name
name = "Zero"

# define a variable call question
question = "Will I find Hercules?"

# store empty string to variable answer
answer = ""

# generating a random number
random_number = random.randint(1, 10)
print(random_number)

# conditions for each randomly generated value
if random_number == 1:
  answer = "Yes - definitely."
elif random_number == 2:
  answer = "It is decidedly so."
elif random_number == 3:
  answer = "Without a doubt."
elif random_number == 4:
  answer = "Reply hazy, try again."
elif random_number == 5:
  answer = "Ask again later."
elif random_number == 6:
  answer = "Better not tell you now."
elif random_number == 7:
  answer = "My sources say no."
elif random_number == 8:
  answer = "Outlook not so good."
elif random_number == 9:
  answer = "Very doubtful."
elif random_number == 10:
  answer = "Signs point to yes."
else:
  answer = "Error."

# print output
print(name + ' asks: ' + question)
print("Magic 8-Ball's answer: " + answer)

# if name is an empty string, print only the question
if name == "":
  print("Question: " + question)
else:
  print(name + ' asks: ' + question)

# question is an empty string, then 8-ball cannot provide a fortune
if question == "":
  print("The Magic 8-Ball cannot provide a fortune unless you ask it something.")
else:
  print(name + " asks: " + question)
  print("Magic 8-Ball's answer: " + answer)
