# Authentication System Task

In this task, we will write a program that receives a table of usernames from the user, generates passwords for them, and then asks them to log in.

## Step 1: Get usernames and passwords

1.  Create a dictionary, `loginInfo`. This will be used to store the usernames and passwords.

2.  Ask for a username for a user.

3.  Generate a random 8-digit code which will be their password. (You will need to use the `randint` function from the `random` library, but make sure that your final 8-digit code is in the form of a string or else the program will not work.)

4.  Add the username and password as a key-value pair to `loginInfo`.

5.  Repeat steps 2-4 until the user enters `"STOP"` as their input for the username.

6.  Iterate through `loginInfo` and print the usernames and their associated passwords.

## Step 2: Ask the user to log in

1.  Repeat the following until three tries have been exhausted:

    a. Ask the user for the username they wish to log in with.
    
    b. Ask the user for the password they wish to log in with.
    
    c. If the username is invalid, the user should receive a message saying so, and continue the loop.
    
    d. If the password is invalid, tell the user so, and continue the loop.
    
    e. If both steps c and d have not continued the loop, tell the user that they successfully logged in and break out of the loop.

2.  After three tries, if the user couldn't successfully get into the authentication system, tell the user so and end the program.

## Sample output

Refer to the following samples to determine how your information will be printed to the user.

### Sample output 1

```console
================
Welcome to the authentication system!
================

Please enter users below to add to the database.

Add user: john123
Add user: admin407
Add user: northsouth2020
Add user: STOP

List of users and passwords:
----------------
john123: 99417261
admin407: 16729101
northsouth2020: 51296501
----------------

================
Sign in page
================

Enter username: billy
================
Welcome to the authentication system!
================

Please enter users below to add to the database.

Add user: john123
Add user: admin407
Add user: northsouth2020
Add user: STOP

List of users and passwords:
----------------
john123: 75873612
admin407: 20963150
northsouth2020: 60079845
----------------

================
Sign in page
================

Enter username: billy
Enter password: 19283712
Invalid username.

Enter username: admin407
Enter password: 88219824
Incorrect password.

Enter username: admin407
Enter password: 20963150
Successfully logged in.
```

### Sample output 2

```console
================
Welcome to the authentication system!
================

Please enter users below to add to the database.

Add user: john123
Add user: admin407
Add user: northsouth2020
Add user: STOP

List of users and passwords:
----------------
john123: 72877386
admin407: 17210930
northsouth2020: 41269279
----------------

================
Sign in page
================

Enter username: john321
Enter password: 81934713
Invalid username.

Enter username: northsouth2020
Enter password: 91827871
Incorrect password.

Enter username: northsouth2020
Enter password: 88827117
Incorrect password.

You have unsuccessfully made 3 attempts to log in. Access denied.
```

