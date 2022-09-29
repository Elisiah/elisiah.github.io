---
layout: post
title:  "Starting the Project"
date:   2022-03-26 16:45:35 +0100
categories: Decompilation
---
<h3>Intro</h3>

For a brief overview, decompilation of N64 games is where all the assembly instructions are rewritten in C code such that we can fully see and understand how every part of the game functions, and change sections much more easily. This is usually done in an effort to allow mods of the game but also will allow us to uncover hidden files and code we have never seen in game.

As I'll reference in a [blog post soon]() I had spent many months delving into the memory of the game Chameleon Twist around 2017.
Initially my goal with reading memory and finding functions was only to find speedrunning skips and so minimal effort
was put in to find anything that couldnt be abused to beat the game faster.

I return to the [Community Discord](https://discord.com/invite/jENRXCfyqq) every now and then to see how chameleon twist speedrunning is going
but this time I saw that [Rainchus](https://github.com/Rainchus) had helped [Nathan R](https://github.com/Nathan-R-Og) with enough information to get a decompilation makefile, that we had spoke about a few timesin the past, into existence. Currently the team includes Rain, Nathan and I - with great help with understanding game structures from Cyanide_Gunner.

Now with a makefile we would be able to rebuild the game if we could convert the game's assembly code into C files. This seemed like a fun challenge which allows me to sharpen my C skills, of which I'm currently taking a University Module in, as well as learn more about MIPS and how N64 games work - which I found a passion for when looking into game memory in the past.

You can keep up with my progress here: [My GitHub Repo for Decompiled C Files](https://github.com/chameleonTwistRet/chameleonTwistv1.0-JP)

<h3>An Example of how decompile matching code works:</h3>

![Assembly Example](/assets/asm_example_1.png){: style="float: left; padding-right: 15px;"}

We start with a .s (MIPS Assembly Instructions) file from the initial Chameleon Twist Makefile Project.

Our goal is then to create a C function that 1:1 matches the assembly instructions of a function (As shown on the left). 

I.e: compiling the C code should return the same instructions as the .s

It is important that it matches 1:1 even if the code is sloppy and could be improved, as rebuilding the game will go through a checksum test.

Once a full C file is made, such that all of its functions one to one match with all .s functions in the same file, we can link the file
and build the game using our code instead of the assembly. This will allow us to modify how the game runs at a later date so people will be able to make their own mods for the game in C code.

There are alot of tricks you quickly pick up on such as: <br>`addiu sp,sp,-0x18` being how much memory space the function reserves on the stack.
By knowing this we can very quickly check if our functions have too many or too few variables in use.

ㅤ<br>
**Here is an example of some C code we may produce (This is the code match of the image left):**

```c
// Author Elisiah (Ellie V)
#define SQ(x) = (x * x)
#define SUM_OF_SQ(x, y) = SQ(x) + SQ(y)

void func_8002D148(float* a, float* b, float c) {
    float sqrtASquaredPlusBSquared;
    float aSquaredPlusBSquared;

    aSquaredPlusBSquared = SUM_OF_SQ(*a, *b);
    if (!(aSquaredPlusBSquared <= SQ(c))) {
        sqrtASquaredPlusBSquared = func_800DB0B0(aSquaredPlusBSquared);    //sqrt func
        *a = (*a * c) / sqrtASquaredPlusBSquared;
        *b = (*b * c) / sqrtASquaredPlusBSquared;
    }
}
```