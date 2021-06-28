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
* Setup.py

* bank_card.tar.gz - zip file containing:
   * Setup.py
   * iduate_bank_card.egg-info (automatically created)
   * dist (automatically created)
   * iduate-bank-card, which contains:

      * BankCard.py - contains methods and attributes for a given bank card
        ** attributes - number, checksum and isValid
        ** methods - luhn_isValid, luhn_checksum
      * setup.cfg
      * README.md
      * license.txt
      * ```__init__.py```

# Installation
pip install iduate-bank-card

# Use
```card1 = BankCard(4417123456789113)```
```f"card number: {card1.number}, is valid: {card1.isValid}, checksum: {card1.checksum}"```


