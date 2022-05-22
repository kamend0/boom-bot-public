# boom-bot Discord bot

A simple Discord bot with two jobs:

* Play noises (mp3 files in the same directory as main.py) when someone enters chat, or on command (!!play clip).
* Announce who enters chat by their Discord name, or by a specified alias.

Please read through main.py for all commands.

To add sounds, create a subdirectory called "sounds" and add sounds as MP3 files; then the Discord bot will refer to them by name: the command "!!play sound" will look for "sound.mp3" in the sounds directory.

To add aliases, create a .py file called "aliases.py" which will contain a dictionary of Discord display name : alias lookups. E.g.: if your friend's Discord display name is 'John' and want his alias to be "JoJo", the dictionary would look like: { 'John' : 'JoJo' }.