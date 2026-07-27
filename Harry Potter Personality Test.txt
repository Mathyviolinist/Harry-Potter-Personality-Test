g = 0
h = 0
r = 0
s = 0

Q1 = int(input('Question 1) How many friends do you have? 1) 0-10, 2) 11-20, 3) 21-30, 4) 31+'))
Q2 = int(input('Question 2) What best describes you? 1) Strong, 2) Strong and Smart, 3) Smart, 4) None of the Above'))
Q3 = int(input('Question 3) What type of activities do you like? 1) Academic, 2) Art and Music, 3) Atheletic, 4) Relaxation'))
Q4 = int(input('Question 4) Are you introverted or extroverted? 1) Introverted, 2) Extroverted, 3) Neither'))

if Q1 == 1:
  r = r + 1
elif Q1 == 2:
  s = s + 1
elif Q1 == 3:
  h = h + 1
elif Q1 == 4:
  g = g + 1
else:
  print('404 ERROR')

if Q2 == 1:
  s = s + 1
elif Q2 == 2:
  g = g + 1
elif Q2 == 3:
  r = r + 1
elif Q2 == 4:
  h = h + 1
else:
  print('404 ERROR')

if Q3 == 1:
  g = g + 1
elif Q3 == 2:
  r = r + 1
elif Q3 == 3:
  s = s + 1
elif Q3 == 4:
  h = h + 1
else:
  print('404 ERROR')

if Q4 == 1:
  r = r + 1
elif Q4 == 2:
  g = g + 1
elif Q4 == 3:
  h = h + 1
  s = s + 1
else:
  print('404 ERROR')
  
print("Gryffindor:", g)
print("Ravenclaw:", r)
print("Hufflepuff:", h)
print("Slytherin:", s)

if g >= r and g >= h and g >= s:
  print('Your house is Gryffindor!')
elif r >= h and r >= s:
  print('Your house is Ravenclaw!')
elif h >= s:
  print('Your house is Hufflepuff!')
else:
  print('Your house is Slytherin!')