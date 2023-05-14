---
layout: post
title:  "Hollow Knight - Cloud Save Downloader"
date:   2022-03-26 16:45:35 +0100
categories: Sideproject
---

<h3>The Problem</h3>
The Xbox Play Anywhere version of Hollow Knight keeps all saves on the cloud as they are technically "xbox saves" and not "pc saves". 

Alot of players wish to move their saves to steam either when their gamepass runs out or when they start speedrunning but since the files are not local they are unable to.

Many player's looking for a solution on blogs and forums were simply told "there wasn't one" but since I had the problem and the skills to solve it I decided to do so.

<h3>Solution:</h3>

I edited the following function from the game such that it would redirect to code for saving locally instead of returning after uploading to the cloud.

Since I do not own the game I will not be posting the full code, however the function changed is as follows:

```c#
// From 0x801633A0
public override void WriteSaveSlot(int slotIndex, byte[] bytes, Action<bool> callback);
```

<h3>A Small Problem</h3>
The `WriteSaveSlot` function takes the `int slotIndex` parameter in order to name the save file. However, the cloud uploading system means that if we locally download a file to a legal slot (1 to 4) then it will be overwritten cloud save data.

<h3>Solution:</h3>

Force the cloud download section of the function to use the harcoded `slotIndex = 5` as it is not used by the game.
