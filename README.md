# Hunar-Intern
#Project 1 (Generating_Captcha)
import string
import random

def generate_captcha(length=5):
    character = string.ascii_letters + string.digits
    captcha=''.join(random.choice(character) for _ in range(length))
    return captcha
captcha = generate_captcha()
print("CAPTCHA:",captcha)
