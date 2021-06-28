# iduate-bank-card Package
Creating package to check if bank card numbers are valid via Luhn Algorithm

# Language
Python

# Files
bank_card.tar.gz

BankCard.py - contains methods and attributes for a given bank card
* attributes - number, checksum and isValid
* methods - luhn_isValid, luhn_checksum

Setup.py

# Installation
pip install iduate-bank-card

# Use
card1 = BankCard(4417123456789113)

f"card number: {card1.number}, is valid: {card1.isValid}, checksum: {card1.checksum}"


