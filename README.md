Objective:
The main objective of this project is to check whether a given password is weak, medium, or strong based on security rules like length, uppercase letters, lowercase letters, numbers, and special characters.
This helps users create strong passwords and improve online security.


🛠️ Tools Used:
Python 3
Built-in re (regular expression) module
IDLE / VS Code / any Python editor

import re

password = input("Enter your password: ")

strength = 0

# check length
if len(password) >= 8:
    strength += 1

# check lowercase
if re.search("[a-z]", password):
    strength += 1

# check uppercase
if re.search("[A-Z]", password):
    strength += 1

# check numbers
if re.search("[0-9]", password):
    strength += 1

# check special characters
if re.search("[@#$%^&*!]", password):
    strength += 1

# result
if strength <= 2:
    print("Weak Password")
elif strength == 3 or strength == 4:
    print("Medium Password")
else:
    print("Strong Password")

    
📌 Conclusion:
This project successfully checks the strength of a password based on multiple security rules. It helps users understand how to create stronger passwords and improve account safety.
This simple project also improves basic Python programming skills like conditions, loops, and string handling.
