# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not

str_pattern = "" 
for row in range(0, 7):    
    for col in range(0, 7):     
        if ((row == 0 or row == 3 or row == 6) and (col > 0 and col < 6)) or ((row == 1 or row == 2) and (col == 0)) or ((row == 4 or row == 5) and (col == 6)):  
            str_pattern += "*"
        else:      
            str_pattern += " "
    str_pattern += "\n"
    
print(str_pattern)

username = input("Enter the username: ")

s = username.lower() 
s = ''.join(char for char in s if char.isalnum())

if s == s[::-1]:
    print("The username is a palindrome.")
else:
    print("The username is not a palindrome.")

