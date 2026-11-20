# Password Security

## Task 1 --- Test a Weak Password

Run:

    echo "password123" | cracklib-check

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/78df2e8d-0670-4a6c-972d-f100dbb3bde0" />


### Questions

1.  What does the tool say about the password?
   ans= It rejects it, saying it is based on a dictionary word.
2.  Why is this password weak?
ans =  It is a common dictionary word with a predictable number added, so attackers can guess it quickly with wordlists and brute force.
### Reflection

Explain why weak passwords are dangerous.
ans= Weak password are easy to guess or crack, which lets attackers take over accounts, steal data and move through a system.
------------------------------------------------------------------------

## Task 2 --- Test a Strong Password

Run:

    echo "Tr4!nBicyclePlanet" | cracklib-check

### Screenshot

<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/a5979a24-e5b5-4745-8f15-aab05f0bc779" />


### Questions

1.  What result did the tool return?
   ans= Ok
2.  What characteristics make this password stronger?
ans= It is long, mixes upper and lower case letter, numbers and a symbol.
### Reflection

Describe at least three characteristics of strong passwords.
ans= Strong passwords are long (12+ characters), mix upper and lower case letter, numbers, symbols.
------------------------------------------------------------------------

## Task 3 --- Password Analysis

Evaluate the following passwords:

-   123456
-   qwerty
-   P@ssword1
-   correcthorsebatterystaple

### Questions

1.  Which passwords are weak?
ans= 123456 and qwerty
3.  Which password is strongest?
   ans=  P@ssword1 and correcthorsebatterystaple

5.  Why?
   ans= P@ssword1 and correcthorsebatterystaple are the strongest because in this password has upper and lower case letter , and numbers, and symbols and long also so it is hard to guess it and 123456 and qwerty these are the weak password because these password can easily guess 
   

### Reflection

Explain what you learned about password strength.
password strength means making the strong password with long (12+ characters), mix upper and lower case letter, numbers, symbols.It helps protect our data and protect our privacy.
