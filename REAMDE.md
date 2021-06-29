# iduate-bank-card package

This packages contains Luhn algorithm results for a given bank card number

# Files

BankCard.py - contains methods and attributes for a given bank card
attributes - number, checksum, isValid and reason
methods - luhn_isValid, luhn_checksum, isValid_reason

# Installation

pip install iduate-bank-card

# Use

card1 = BankCard(4417123456789113)
f"card number: {card1.number}, is valid: {card1.isValid}, reason: {card1.reason}, checksum: {card1.checksum}"

card2 = BankCard(141)
f"card number: {card2.number}, is valid: {card2.isValid}, reason: {card2.reason}, checksum: {card2.checksum}"
