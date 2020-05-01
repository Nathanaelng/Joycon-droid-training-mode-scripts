# JOYCON DROID TRAINING MODE SCRIPTS

These are scripts for the Tas UI feature in Joycon droid that can be downloaded from the Play Store.

Things to note when using the scripts.

-Not every script is optimised as sometimes tje cpu will do something that isnt exactly intended to happen as I'm still trying to learning how to write these the best I can.

-When using scripts to make the cpu DI they occasionally do no DI.

-Landing aerials arent done close enough to the ground where they are the safest due to latency issues with the app.

-Some characters fall too fast so the wont be able to read the attack input reliable before or after the fast fall input like wolf so I chose to just do regular FH wolf nairs instead. Once the app gets better I'll write one for FHFF Wolf Nair.

-If you are practicing parrys, the  cpu will stop and try to jab straight afterward usually.

-If there are any issues with the script you can usually just reset training mode and then just wait for a few runs of the script.

-Included cloud side b to practice parrying on cause wifi cloud is something we all have to worry about during these dark times.

App is still in alpha so if you want to write something that is smaller than a 5 frame window, then it most likely wont be possible as of now.

If you have any issues you can DM me on twitter or even better you can join joycon droids discord server ask questions here https://discord.gg/xsHHsh3

________________________________________________________________________________________________________________________________________


IF YOU WANT TO WRITE YOUR OWN

-The format of a line of a script is as follows:

[frame number] [list of keys to press, separated by semicolons] [x and y coordinates of the left joystick, sparated by a semicolon] [x and y coordinates of the right joystick, separated by a semicolon]

Note: The x and y coordinates should range from the value -30000 to 30000.

The list of keys is as follows: KEY_A, KEY_B, KEY_X, KEY_Y, KEY_LSTICK, KEY_RSTICK, KEY_L, KEY_R, KEY_ZL, KEY_ZR, KEY_PLUS, KEY_MINUS, KEY_DLEFT, KEY_DUP, KEY_DRIGHT, KEY_DDOWN

The keys must be spelled EXACTLY like this or else it will not register. To press no keys on a frame, simply put NONE.

You only need to specify frames where there are inputs as the program will default to nothing pressed on a frame. However, if you specify one part, you must specify all of them per frame (ex. if you only want to press the A button, you still need to tell the program that the analog sticks are to be at pos 0;0 and 0;0).

If you want to make the CPU press 2 buttons at the same time, just seperate the 2 keys with (;). Ie. KEY_Y;KEY_A
