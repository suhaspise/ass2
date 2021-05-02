
import random
name=input("what is your name?")
print("ALL THE BEST!!",name)
data=['computer','java','python','programming','condition']
word=random.choice(data)
print("guess the word")
guesses=''
turns=12
while turns>0:
    
    failed=0
    
    
    
    for char in word:
        if char in guesses:
            print(char)
        else:
            
            print("-")
            
            failed+=1
            
    if failed==0:
   
        print("!!YOU WIN!!")
        print("The word is:",word)
        break
    guess=input("guess a character ")
    
    guesses+=guess
    
    if guess not in word:
        turns-=1
        print("wrong")
        print("You have",+turns,'more guesses')
        if turns==0:
            print("!!YOU LOOSE!!")
    
        
 output:



what is your name? Krushna
ALL THE BEST!!  Krushna
guess the word
-
-
-
-

guess a character j
j
-
-
-

guess a character a
j
a
-
a

guess a character v
j
a
v
a
!!YOU WIN!!
The word is: java




what is your name? Suhas
ALL THE BEST!!  Suhas
guess the word
-
-
-
-
-
-
-
-

guess a character c
c
-
-
-
-
-
-
-

guess a character i
wrong
You have 11 more guesses
c
-
-
-
-
-
-
-

guess a character n
wrong
You have 10 more guesses
c
-
-
-
-
-
-
-

guess a character e
c
-
-
-
-
-
e
-

guess a character m
c
-
m
-
-
-
e
-

guess a character a
wrong
You have 9 more guesses
c
-
m
-
-
-
e
-

guess a character t
c
-
m
-
-
t
e
-

guess a character h
wrong
You have 8 more guesses
c
-
m
-
-
t
e
-

guess a character e
c
-
m
-
-
t
e
-

guess a character a
wrong
You have 7 more guesses
c
-
m
-
-
t
e
-

guess a character t
c
-
m
-
-
t
e
-

guess a character e
c
-
m
-
-
t
e
-

guess a character r
c
-
m
-
-
t
e
r

guess a character f
wrong
You have 6 more guesses
c
-
m
-
-
t
e
r

guess a character o
c
o
m
-
-
t
e
r

guess a character r
c
o
m
-
-
t
e
r

guess a character m
c
o
m
-
-
t
e
r

guess a character o
c
o
m
-
-
t
e
r

guess a character i
wrong
You have 5 more guesses
c
o
m
-
-
t
e
r

guess a character v
wrong
You have 4 more guesses
c
o
m
-
-
t
e
r

guess a character e
c
o
m
-
-
t
e
r

guess a character s
wrong
You have 3 more guesses
c
o
m
-
-
t
e
r

guess a character s
wrong
You have 2 more guesses
c
o
m
-
-
t
e
r

guess a character f
wrong
You have 1 more guesses
c
o
m
-
-
t
e
r

guess a character g
wrong
You have 0 more guesses
!!YOU LOOSE!!
