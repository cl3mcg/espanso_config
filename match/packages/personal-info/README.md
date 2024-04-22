# Espanso Personal Information Package

## Introduction

The 'personal-info' package is a private repository meticulously crafted to safeguard your sensitive information. It is strongly advised not to share or publish this package online.

- Full name formatted correctly.
- Email addresses formatted accurately.
- Phone numbers formatted properly.

In the interest of security and privacy, no supplementary information is retained in this package.

This package is particularly beneficial for individuals with complex or lengthy names, or names that include special characters, making them difficult to input using a conventional English QWERTY keyboard.

## Setup

1. Generate a file named `package.yml`.
2. Create a `.gitignore` file in the root directory of your Espanso configuration folder to prevent the `package.yml` file from being monitored by your version control system.
3. Input the required data to be auto-filled. Here's a basic template that can be expanded with additional commands:

```yaml
matches:
  # Full name output
  - triggers: ["name\t", "::name"]
    replace: "Odile DERAY"
    label: "Output full name with accents"

  # Professional email greeting
  - triggers: ["hp\t", "::hp"]
    replace: "Hello,\nI am Odile DERAY, a press officer based in Cannes, France. I hope this message finds you well.\nI am reaching out to you because "
    label: "Output professional email introduction"

  # Professional email address output
  - triggers: ["empro\t", "::empro"]
    replace: "odile_deray@press.com"
    label: "Output professional email address"
```
