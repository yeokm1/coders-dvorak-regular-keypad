# programmer-dvorak-normal-keypad

I like [Roland Kaufmann's Programmer Dvorak](http://www.kaufmann.no/roland/dvorak/) keyboard layout however I dislike the fact that he reverses the direction of the numeric keypad. This is an installable solution that slightly backtracks from his improvements.

To get an idea, here is a comparison

![Screen](images/original-programmer dvorak.png)

Kaufman's original layout with "improved" keypad layout

![Screen](images/unicomp-spacesaver-104.jpg)

My normal keypad version

If you prefer my version, continue on.

##How to use?

1) Go to the [Releases](https://github.com/yeokm1/programmer-dvorak-normal-keypad/releases) section.  
2) Download either the "English Singapore" or "English US" version relevant to your operating system Windows/Mac.  
3) Unzip the file  

###Windows
3) Run `msi` or `setup.exe`  
4) Go to Control Panel -> Language  
5) Select your language -> Option -> Add an input method   
6) Search for `Programmer Dvorak - Normal Keypad` and Add. If the new layout is not visible, you may need to reboot your machine and start from Step 4.

###Mac
3) Copy the bundle file to `/Library/Keyboard Layouts` if you want it to be system wide or `~/Library/Keyboard Layouts` if you only want it for the current user.  
4) Go to System Preferences, Keyboard, Input Sources, click "+", select English, select `Programmer Dvorak - Normal Keypad`

###For Login Screen
This above settings are only tied to your user account, to set it as the default for the login prompt, visit these links:  
[For Mac](http://www.macissues.com/2015/04/16/fix-an-incorrect-default-keyboard-layout-at-the-os-x-login-prompt/)

The simplest option stated in the link above is to relauch the Setup Assistant:

1. Run `sudo rm /var/db/.AppleSetupDone` in Terminal
2. Restart your Mac
3. Set your new keyboard layout when asked to do so
4. You will come to a point where you have to create a new user account. I just created a dummy account to prevent conflicts with my existing username.
5. Once you have logged in, you can delete the dummy account.

[For Windows](https://social.technet.microsoft.com/Forums/windows/en-US/c64ee221-db3c-4058-8d1b-673de613535f/how-to-change-keyboard-layout-for-login-and-password-in-windows-8?forum=w8itprogeneral)

Go to Control Panel:
"Open "region" > then on the "administration" tab > click "copy settings" > then check the box "for home screen & new users"."

##How to modify?

If you need to modify the layout for some reason...

###Windows

1) Install the [Microsoft Keyboard Layout Creator](https://msdn.microsoft.com/en-us/goglobal/bb964665.aspx)  
2) Open the `.klc` file you wish to modify. I can't seem to view the keypad in MKLC though. 

You should see something like this:  

![Screen](images/windows-prod-dvorak-main.png)

![Screen](images/windows-prod-dvorak-shift.png)

3) Set current working directory  
4) Once you are done, click Project->Build DLL and Setup Package.  
5) Go to your working directory to retrieve the install folder  

###Mac

1) Install [Ukelele](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=ukelele)  
2) Open the `.keylayout` file you wist to modify. You may wish to change the keyboard type to view the keypad. View -> Keyboard Type -> Third party.

You should see something like this:  

![Screen](images/mac-prod-dvorak-main.png)

![Screen](images/mac-prod-dvorak-shift.png)

3) Save as bundle
