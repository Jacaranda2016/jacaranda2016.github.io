## Use cases
Sometimes we need to input the password and do not want it to echo the password to the console. For example, if we use Jupyter for the scriping,
it would be not safe if we type the password and echo it to the console. 

## Solution-- Python getpass

Many programs that interact with the user via the terminal need to ask the user for password values,
without showing what the user types on the screen. The _getpass_ module provides a portable way to 
handle such password security.

The _getpass()_ function prints a prompt then reads input from the user until they press return. 
The input is passed back as a string to the caller. 
'''
import getpass
user=getpass.getuser() #return the username of the OS
password=getpass.getpass("Password")
'''

## the encoding requirement for URLs
Some characters have special meanings in URL such as "&" and "=". So if you have such kinds of characters in your password, you need 

## Password Security
