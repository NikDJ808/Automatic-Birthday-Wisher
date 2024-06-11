# Birthday Wisher

Welcome to the Birthday Wisher project! This repository contains the code for an automated birthday wisher application. The application is designed to send personalized birthday wishes to your friends and family on their special day. It reads birthday data from a CSV file, selects a template, and sends the email using Python.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Files](#files)

## Introduction

The Birthday Wisher is a Python-based application that automates the process of sending birthday wishes. By keeping a CSV file with birthday information, the application checks daily for any birthdays and sends a personalized email using one of the provided templates.

## Features

- Automatically send birthday wishes via email
- Personalized messages using templates
- Easy-to-update CSV file for managing birthdays
- Customizable email content

## Installation

To run the Birthday Wisher, you need to have Python installed on your system. Follow these steps to set up the application:

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/birthday-wisher.git
   ```

2. Navigate to the project directory:
   ```sh
   cd birthday-wisher
   ```

3. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Usage

To start the application, run the main Python script:

```sh
python main.py
```

Make sure to update the `birthdays.csv` file with the relevant information. The CSV file should have the following columns:

- `name`: Name of the person
- `email`: Email address of the person
- `year`: Birth year
- `month`: Birth month
- `day`: Birth day

The application will check for today's date and send a personalized birthday wish using one of the templates found in the `letter_templates` directory.

### Email Setup

Before running the script, make sure to configure your email settings in the `main.py` file:

```python
my_email = "your_email@example.com"
password = "your_email_password"
```

Ensure you have allowed less secure apps or used an app-specific password if required by your email provider.

## Files

The repository contains the following key files:

- `main.py`: The main script to run the birthday wisher.
- `birthdays.csv`: The CSV file containing birthday information.
- `letter_templates/letter_1.txt`: Template for birthday wish 1.
- `letter_templates/letter_2.txt`: Template for birthday wish 2.
- `letter_templates/letter_3.txt`: Template for birthday wish 3.
