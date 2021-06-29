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

* pipy_upload_terminal_commands.rtf
```
python3 setup.py sdist bdist_wheel
pip install twine

# commands to upload to the pypi test repository
twine upload --repository-url https://test.pypi.org/legacy/ dist/*
pip install --index-url https://test.pypi.org/simple/ iduate-bank-card

# command to upload to the pypi repository
twine upload dist/*
pip install iduate-bank-card
```

* iduate_bank_card.tar.gz - zip file containing:
   * Setup.py
   * iduate_bank_card.egg-info (automatically created)
   * dist (automatically created)
   * build (automatically created)
   * iduate-bank-card, which contains:

      * BankCard.py - contains methods and attributes for a given bank card
         * attributes - number, checksum, isValid and reason
         * methods - luhn_isValid, luhn_checksum, isValid_reason
      * setup.cfg
      * README.md
      * license.txt
      * ```__init__.py```
      * ```__pycache__```

# Installation
pip install iduate-bank-card

https://pypi.org/project/iduate-bank-card/

# Use
```
>>> from iduate_bank_card import BankCard
>>> card1 = BankCard(4417123456789113)
>>> f"card number: {card1.number}, is valid: {card1.isValid}, reason: {card1.reason}, checksum: {card1.checksum}"
'card number: 4417123456789113, is valid: True, reason: checksum, checksum: 70'
>>> card2 = BankCard(141)
>>> f"card number: {card2.number}, is valid: {card2.isValid}, reason: {card2.reason}, checksum: {card2.checksum}"
'card number: 141, is valid: False, reason: Number does not meet minimum requirements, checksum: 10'
```


