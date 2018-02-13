# About me
Hi there! i'm Soulaimane Ech Charaouy, a communication and Multimedia Design student and for an assignment we had to work with dotfiles.

# Installation
First of all you need to have a ```.bash_profile``` or ```.profile``` in your user directory. You can
check if you have one by going to your user directory ```cd ~``` and look at all the files
by typing ```ls -a.``` If you don't have a .bash_profile or .profile file yet you have to make
one: ```touch .bash_profile```.

## Aliases
The first thing i did was creating a few basic aliases. You have to put the aliases in your ``` .bash_profile ```
, you can get in this file by typing ```nano .bash_profile``` or open the file in your text
editor. After that it is pretty simple you put ```alias``` and the shortcut you want to make for example:
`` alias cd..="cd .." ``

**Note**: Dont put a space before or after the ``=``, the alias will not work if you do this.


## Prompt
After the aliases I modified my prompt. I did this again in ``nano .bash_profile``, the code to modify your prompt is ``PS1=""``. What you put between ``""`` depends on what you want to modify, for example I wanted it to show a trophy emoji, date, time and my name so my code looked like this `` PS1="🏆 \[\d \A] \u \$ "``.
I found the shortcuts like ``/u``, what stands for username, on [this site](https://www.howtogeek.com/307701/how-to-customize-and-colorize-your-bash-prompt/), take a look because there are a lot more things you can customize the prompt with!

## Welcome Message
As a welcome message my terminal shows me the weather in Amsterdam. You can do this by putting ``curl wttr.in/Amsterdam?0q`` in your .bash_profile.


## theFuck
If you are someone who makes a lot of typo errors this is perfect for you. What fuck does is correcting your previous console command and it is quiet easy to Install. You first need to install Homebrew, after you installed Homebrew you can use ``brew install thefuck`` to install thefuck. After that you put ``alias fuck='$(thefuck $(fc -ln -1))'`` in your ``.bash_profile`` file and you are good to go!
