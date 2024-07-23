### Password Generator ###

import secrets
import string

def password():
    lowercase = string.ascii_lowercase
    uppercase = string.ascii_uppercase
    digits = string.digits
    symbols = string.punctuation
    alphabet = lowercase + uppercase + digits + symbols

    password_length = int(input("Enter your new password's length (between 8 and 16 characters): "))
    while password_length < 8 or password_length > 16:
        if password_length < 8:
            print("Error: the entered number is smaller than the recommended size")
            password_length = int(input("Enter your new password's length (between 8 and 16 characters): "))
        elif password_length > 16:
            print("Error: enter a number between 8 and 16")
            password_length = int(input("Enter your new password's length (between 8 and 16 characters): "))

    password = ""
    for i in range(password_length):
        password += "".join(secrets.choice(alphabet))
    return password


new_password = password()
print("Your new password is:", new_password)
