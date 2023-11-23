PWD_Security by @Joelbu537

I created this C# program to test stuff related to safely storing passwords.
The program consists of a login page and nothing more, because I wasn't creative enough to make an actual application where you can log in and do stuff.
Now you have this: A simple login/sign up program

Features/explanation:
 - You can create/login-to accounts. Accounts consist of an username and a password.
 - All data is stored in \data\userdata.bin
 - Passwords are salted and hashed to guarantee safety for users and headaches for programmers trying to understand the algorythm I built.
 - Passwords are never displayed in plaintext, the shown characters are replaced by *'s.
 - I made the program pretty idiot-secure so you can't log into accounts that don't exist or just use the first half of a password to trick the algorithm into thinking its the true password
   (This was an actual bug where the program would only check the first character of the pwd and then REPLACE the stored hash with this FUCKING CHARACTER. which of course made the account unaccesable
 - It's console based yay:D
 - The ammount of saved accounts is capped at 1000 because I was too lazy to use different files or some other strategy change it yourself
