---
layout: post
title:  "Unlocking the Debug Menu"
date:   2022-08-24 14:40:22 +0100
categories: Decompilation
---
*Please note this article contains information on Chameleon Twist as a whole but will only be written pertaining to the JP v1.0 ROM*

<h2>Intro</h2>

For players of retro games such as speedrunners finding a debug menu is like the holy grail. It can be useful for learning new things about the game, its another fact we can add to our repetoir that no one will ever ask us about and like the holy grail there is a chance you will never find it.

When going through dissasembled code for the Chameleon Twist Decompilation Project[] it was noticed that a certain function was checking for values of `0x800` `0x400` `0x200` and `0x100` respectively. Having written input handling assembly code for the N64 in the past these stood out as the User's DPAD Input Buttons. 

#

<h3>Unlocking the Menu</h3>

Unfortunately, Nathan found that the addresses themselves are never checked as the developer's put an impossible conditional statement to stop them running in the game's official release. But by simply `NOP` valuing the instruction to check this conditional. We can input the sequence ` Hold L + {D-UP, D-DOWN, D-LEFT, D-RIGHT}` to activate the debug menu flag.

For those who cannot edit the game's code itself I have created N64 cheat codes which can be used inside emulators or even on the system if you have the GameGenie (this skips the step of inputting the sequence):
```
// Name: Debug Flag Activation
// Author Ellie V.

800F06B0 0000
800F06B1 0000
800F06B2 0000
800F06B3 0001
```

<h2> Using the Menu </h2>
<h3> I. Reading the Menu </h3>
<h3> II. Movement and Noclip </h3>
<h3> II. Changing the Camera </h3>