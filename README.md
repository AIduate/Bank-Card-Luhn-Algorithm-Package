## Table of contents
* [Introduction](#introduction)
* [Languages](#languages)
* [Files](#files)
* [Installation](#installation)
* [Use](#use)

# Introduction
Creating package to check if bank card numbers are valid via Luhn Algorithm using object oriented programming and uploading to pypi test and prod

# Languages
* Python
* Bash

# Files
Setup.py

bank_card.tar.gz - zip file containing the following:

BankCard.py - contains methods and attributes for a given bank card
* attributes - number, checksum and isValid
* methods - luhn_isValid, luhn_checksum

# Installation
pip install iduate-bank-card

# Use
card1 = BankCard(4417123456789113)

f"card number: {card1.number}, is valid: {card1.isValid}, checksum: {card1.checksum}"


