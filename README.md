Pikapy - [NOT DEAD READ BELOW] Mass Pokemon Go Account Creator and ToS verifier
==============================================================

#NOTICE
##DUE TO NIANTIC IMPLEMENTING RECAPTCHA IN THE SIGN-UP PROCESS, THIS SCRIPT IS NOT WORKING ANYMORE. BUT ITS NOT THE END, READ BELOW
#### Niantic has implemented reCaptcha into their signup process, causing this script to stop working. But we are working on a website which will allow you generate accounts just with a few clicks!

Description
-----------
Automatically creates Pokemon Trainer Club accounts, and reads the ToS making them usable after the recent Niantic patch.
Text files will be created in your current directory. 

usernames.txt will give the needed output for https://github.com/favll/pogom in username:password format.

Installation
------------

Note: If you are upgrading from the last version, you will have to update and/or reinstall the requirements.

Install from Github using pip::

    pip install git+https://github.com/skvvv/pikapy
    
If given errors try (Due to both having python2 and python3):
    
    pip2 install git+https://github.com/skvvv/pikapy  
    
Or if given permission errors:

    sudo pip2 install git+https://github.com/skvvv/pikapy  

If given error:

    from pgoapi import PGoApi
    ImportError: No module named pgoapi
    
Run:

    pip install git+https://github.com/keyphact/pgoapi.git

If you are having problems with installation, join us on https://discord.gg/2cmhB

Use
---
**Command line interface:**

After installing the package run 'pikapy' from the terminal to create a new accounts.
Optional parameters include *--username*, *--password*, *--email*, *--count*
Use *--help* for command line interface help.

Example 1 (Create entirely random new account)::

    ~pikapy
    Created new account:
      Username:  dGXJXnAzxqmjbaP
      Password:  yUbiAgcXhBrEwHk
      Email   :  TVKzlu1AcW@6yxi6.com
      
Example 2 (Create 2 accounts with the same password)::

    ~pikapy -p password -c 2
    Created new account:
      Username:  dGXJXnAzxqmjbaP
      Password:  password
      Email   :  TVKzlu1AcW@6yxi6.com
    Created new account:
      Username:  vKEkp19eb0l4mFW
      Password:  password
      Email   :  TVKzlu1AcW@6yxi6.com
      
Example 3 (Create a new account with specified parameters)::

    ~pikapy --username=mycustomusername --password=hunter2 --email=verifiable@lackmail.ru
    Created new account:
      Username:  mycustomusername
      Password:  hunter2
      Email   :  verifiable@lackmail.ru


Extra Options:

- *--email-tag*: Add the username as a tag to the email (e.g. address+username@gmail.com)
Output is saved both as a list of usernames, and pokemongo-map ready -u username1 -u username2 -username3... format

    

