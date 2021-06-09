# PyPassword_Generator

## A simple but strong password generator using python that create strong custom password based on your need

## Program

    import random
    
    print("Welcome TO PyPassword Generator")
    print("-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-")

    l = int(input("\nHow many letters do you need in the pass    :"))
    n = int(input("How many numbers do you need in the pass    :"))
    c = int(input("How many characters do you need in the pass :"))
    print("----------------------------------------------\n")

    letters ='qwertyuiopasdfghjklzxcvbnm'
    numbers ='1234567890'
    chara ='!@#$%^&*()_+[]{}<>,.?;:'
    passw =[]
    password=''

    for i in range (0,l):
      passw.append(random.choice(letters)) 

    caps =random.randint(1,l)
    for ca in range(0,caps-1):
      passw[ca] = passw[ca].upper()

    for j in range (0,n):
      passw.append(random.choice(numbers))

    for k in range (0,c):
      passw.append(random.choice(chara))

    random.shuffle(passw)
    for z in passw:
      password += z
    print(f"Your Paswword is :{password}")
    
## Output

    Welcome TO PyPassword Generator
    -*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-
    
    How many letters do you need in the pass    :5
    How many numbers do you need in the pass    :4
    How many characters do you need in the pass :4
    ----------------------------------------------

    Your Paswword is :$W57e(7^.N0fI




