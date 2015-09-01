JBot
----
Telegram Bot that dose everything!


features:
---------
 * easy to add abilities
 * highly customizable command framework
 * fully multithreaded

Supports:
--------
Python2 and Python3

Dependencies:
-------------
python-telegram-bot  
praw  
wikipedia  
requests  
futures

Basic setup and installation:
-----------------------------
 In conf/configuration.py fill your telegram token.  
 Import and add the desired abilities to the abilities set

 set your telegram bot to "privacy false" with BotFather (/setprivacy false)

 clone the project, create virtualenv and install dependencies  
 
        pip install -r requirements.txt
 run the bot
 
        python main.py

bot usage:
----------

The bot will only answer when addressed with one of the words that are contained in BOT_ADDRESS_SET
for example:  

        yo j

after the bot address, a command should follow:

        yo j wiki robots

the commands are registered throw each ability, see abilities dir for examples.

if the command is found JBot will run the method with which the command is registered to.


plans for the future:
---------------------
 * isolate the replies per message id
 * simplify command decorator
 * improve command framework
 * create full bot framework
 * add tests
 
  
License
----

MIT
