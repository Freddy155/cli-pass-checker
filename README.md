CLI Password Strength Checker
=======================================

Introduction
------------

The Password Strength Checker is a Python script designed to evaluate the strength of a given password based on various criteria, including the presence of lowercase letters, uppercase letters, digits, whitespaces, and special characters. It calculates a score for the password and provides remarks on its strength.

Table of Contents
-----------------

-   [Installation](#installation)
-   [Usage](#usage)
-   [Code Explanation](#code-explanation)

Installation
------------

To use the Password Strength Checker, you'll need to follow these steps:

1.  Clone the GitHub repository to your local machine. Use the following command in your terminal:

    ```bash
    git clone https://github.com/Freddy155/cli-pass-checker.git
    ```

2.  Make sure you have Python installed on your system.

3.  Navigate to the project directory:

    ```bash
    cd cli-pass-checker
    ```


4.  Run the script:

    ```bash
    python app.py
    ```

The script will prompt you to enter a password and provide feedback on its strength.

Usage
-----

Here's how you can use the Password Strength Checker:

1.  Run the script by executing `app.py` in your terminal.

2.  You'll be prompted to enter a password. The input is hidden for security reasons.

3.  The script will evaluate the password and provide the following information:

    -   Number of lowercase letters
    -   Number of uppercase letters
    -   Number of digits
    -   Number of whitespaces
    -   Number of special characters
    -   Password score (on a scale of 1 to 5)
    -   Remarks on the password's strength
4.  You can choose to check another password's strength or exit the program.

Code Explanation
----------------

The script consists of the following functions:

-   `check_password_strength()`: This function calculates the strength of the entered password by analyzing its character composition. It then provides remarks based on the password's strength.

-   `check_pwd(another_pw=False)`: This function handles user input to decide whether to check another password's strength or exit the program.

The main block of the script welcomes the user and initiates the password strength checking process.

### Password Strength Scale

-   1: Very bad password. Change it as soon as possible.
-   2: Weak password. Consider using a tougher password.
-   3: Password is okay but can be improved.
-   4: Hard to guess password, but further improvements are possible.
-   5: Extremely strong password. Hackers don't stand a chance.

Example
-------

```bash
python app.py
```


Output:

```python

===== Welcome to Password Strength Checker =====
Do you want to check your password's strength (y/n) : y
Enter the password:
Your password has:-
1 lowercase letters
1 uppercase letters
1 digits
0 whitespaces
1 special characters
Password Score: 1.0
Remarks: That's a very bad password. Change it as soon as possible.
Do you want to check another password's strength (y/n) : n
Exiting...

```