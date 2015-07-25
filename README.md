# programmer-dvorak-normal-keypad

I like [Roland Kaufmann's Programmer Dvorak](http://www.kaufmann.no/roland/dvorak/) keyboard layout however I dislike the fact that he reverses the direction of the numeric keypad. This is an installable solution that sort of backtracks from his improvements.

To get an idea, here is a comparison

![Screen](images/original-programmer dvorak.png)

Kaufman's original layout with "improved" keypad layout

![Screen](images/unicomp-spacesaver-104.jpg)

My normal keypad version

If you prefer version, continue on.

##How to use?

1) Go to the [Releases](https://github.com/yeokm1/programmer-dvorak-normal-keypad/releases) section.  
2) Download either the "English Singapore" or "English US" version relevant to your operating system Windows/Mac.  
3) Unzip the file  

###Windows
3) Go to Control Panel -> Language  
4) Select your language -> Option -> Add an input method   
5) Search for `Programmer Dvorak - Normal Keypad` and Add. If the new layout is not visible, you may need to reboot your machine and start from Step 3.

###Mac
3) Copy the bundle file to `/Library/Keyboard Layouts` if you want it to be system wide or `~/Library/Keyboard Layouts` if you only want it for the current user.  
4) Go to System Preferences, Keyboards, Input Sources

##How to modify?

If you need to modify the layout for some reason...

###Windows

1) Install the [Microsoft Keyboard Layout Creator](https://msdn.microsoft.com/en-us/goglobal/bb964665.aspx)  
2) Open the `.klc` file you wish to modify. You should see something like this:  


![Screen](images/windows-prod-dvorak-main.png)

![Screen](images/windows-prod-dvorak-shift.png)

3) Set current working directory  
4) Once you are done, click Project->Build DLL and Setup Package.  
5) Go to your working directory to retrieve the install folder  

###Mac

1) Install [Ukelele](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=ukelele)  
2) Open the `.keylayout` file you wist to modify. You should see something like this  
3) Save as bundle
