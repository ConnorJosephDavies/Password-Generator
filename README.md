# Password Generator

A desktop app for generating random passwords. Choose a strength, how many digits and special characters you want, and the password is copied to your clipboard.

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ConnorJosephDavies/ConnorJosephDavies/main/assets/password-generator-dark.svg" />
    <img src="https://raw.githubusercontent.com/ConnorJosephDavies/ConnorJosephDavies/main/assets/password-generator-light.svg" alt="Password Generator app window" width="520" />
  </picture>
</p>

## Features

- Three strength levels: **Weak** (8 characters), **Strong** (10) and **Very Strong** (12)
- Sliders for the number of digits and special characters
- Optionally start the password with a letter of your choice
- The generated password is copied to your clipboard automatically

## Built with

- **Python 3**
- **PyQt5** for the interface
- Python's `random` and `string` modules to build the password

## Getting started

```bash
git clone https://github.com/ConnorJosephDavies/Password-Generator.git
cd Password-Generator
pip install PyQt5
python password_generator.py
```

## A note on security

This project uses Python's `random` module, which is fine for learning but isn't designed for security. For real passwords, Python's `secrets` module is the recommended choice. Switching to it is on the list below.

## Ideas for improvement

- Use the `secrets` module instead of `random`
- Let the user choose any password length
- Add a strength meter
- Clear the clipboard after a short time