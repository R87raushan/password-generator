# Password Generator in Python

import random
import string

print("===== PASSWORD GENERATOR =====")

# User se password length lena
length = int(input("Enter password length: "))

# Characters set
letters = string.ascii_letters
digits = string.digits
symbols = string.punctuation

# Sabhi characters ko combine karna
all_characters = letters + digits + symbols

# Random password generate karna
password = ""

for i in range(length):
    password += random.choice(all_characters)

# Output
print("\nGenerated Password:", password)
