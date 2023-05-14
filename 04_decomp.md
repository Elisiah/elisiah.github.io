---
layout: page
title: Decompilation
permalink: /decomp/
---
![](https://img.shields.io/badge/-C-navy)
![](https://img.shields.io/badge/-Python-blue)
![](https://img.shields.io/badge/-MIPS%20Assembly-yellow)

<h2>Overview</h2>
The Chameleon Twist Decompilation Project is a multi-year project, started on Mar 27, 2022, to rewrite the Nintendo 64 games Chameleon Twist 1 and 2 in C. 

The games were originally written in C and compiled to MIPS assembly using an IDO compiler. The project aims to reverse engineer the assembly code so that we may write our own C code that builds an identical game. 

The project is hosted on GitHub and is open source. It is currently being worked on primarily by 3 people with help from other N64 decompers.

<img src="https://github.com/chameleonTwistRet/chameleonTwistv1.0-JP/actions/workflows/ci.yml/badge.svg"> 
<img src="https://img.shields.io/endpoint?label=Code%20JP&url=https%3A%2F%2Fprogress.deco.mp%2Fdata%2Fchameleontwist%2Fjp%2Fdefault%2F%3Fmode%3Dshield%26measure%3Dfuncs&color=yellow"/> <img src="https://img.shields.io/endpoint?label=All%20JP&url=https%3A%2F%2Fprogress.deco.mp%2Fdata%2Fchameleontwist%2Fjp%2Fdefault%2F%3Fmode%3Dshield%26measure%3Dbytes&color=orange"/>

<h2>Offshoot Projects</h2>
<h3><a href="/decompilation/2023/03/10/ctBlend.html">ctBlend</a></h3>
- There is an, as yet unpublished, blender tool being worked on by me and another member of the team to allow for the creation of custom levels for Chameleon Twist 1.

<h2>Languages and Skillset</h2>

<b>C</b>: Our source code for the game is written in C so it is used for the majority of the project; in addition the N64 sdk is written in C so we use it to interface with the hardware. Modifications for the game also now use C.

<b>Python</b>: Our buildsystem for the rom uses ninja. In addition, we mainly use python to create tools to aid in the reverse engineering process.

<b>MIPS Assembly</b>: The N64 is a MIPS based system so we need a good understanding of MIPS assembly to reverse engineer the game. Further, earlier on in the project we had write MIPS asm to create hooks for modifications to the gameas well as for the modifications themselves.