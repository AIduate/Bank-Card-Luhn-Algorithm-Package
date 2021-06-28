# iduate_bank-card package

This packages contains Luhn algorithm results for a given bank card number

# Files

BankCard.py - contains methods and attributes for a given bank card
attributes - number, checksum and isValid
methods - luhn_isValid, luhn_checksum

# Installation

pip install bank-card

# Use

card1 = BankCard(4417123456789113)
f"card number: {card1.number}, is valid: {card1.isValid}, checksum: {card1.checksum}"
