---
description: How to create your V as an NPC
---

# NPV - V as custom NPC

**Created by @manavortex**\
**Published May 13 2023**

This guide will show you how to do the following things:&#x20;

* Setting up a Wolvenkit project with the prepared example files
* Creating your V's head in Blender (has its own [sub-page](npv-preparing-the-head-in-blender.md))
* Adding them as an NPC to spawn them with AppearanceMenuMod (has its own sub-page)

#### Difficulty:

Easy, but not trivial: you don't need any prior knowledge, but the whole structure is complex, and if you make mistakes, you will end up missing files.

**It uses the following versions:**

* Cyberpunk 2077 game version >= 1.6
* [WolvenKit](https://github.com/WolvenKit/Wolvenkit/releases) >= 8.9.0
* [Blender](https://www.blender.org/download/) 3.5.1&#x20;
* [AppearanceMenuMod](https://www.nexusmods.com/cyberpunk2077/mods/790) >= 2.1

{% hint style="info" %}
For the community guides on the same topic together with many extra guides and resources, see [here](https://wiki.redmodding.org/cyberpunk-2077-modding/modding-guides/community-guides/npvs-v-as-npc-custom-npcs).&#x20;
{% endhint %}

{% hint style="warning" %}
None of this would have been possible without **NoraLee**, who pioneered the process and taught me everything that I needed to know to set up these tools. This guide doesn't use any of her resources, but a lot of her knowledge. For her full guide with all edge-cases, bells, whistles and context, see her [Google Drive](https://drive.google.com/drive/folders/1R-knopKMhHDZuokPKaTt0nIDArXcQdrb).&#x20;

This is the speedrun version. If you want extra details and context, please check Nora's Google Doc.
{% endhint %}

## Preparation

I have prepared an example project ([mana's mega](https://mega.nz/file/aVETXTaB#gqKTnP\_lBNxe0b1w9b8TM5agENIIIAAxyLmMd8Kb6l8) | Nexus) for you again, but due to the complexity of V's head mesh, you have to do a little bit of prep work here.

Don't worry, I'll walk you through it step by step.

### The character preset

To create a face, we need to know the following numeric values from the character creator:&#x20;

* Eyes
* Eyebrows
* Nose
* Mouth
* Jaw
* Ears

Find the mirror in V's apartment and note them down, or load a savegame in [Cybercat](https://www.nexusmods.com/cyberpunk2077/mods/718).

### Setting up the files

{% hint style="info" %}
**Body gender:**

As a rule of thumb, I'll document the process for an NPV with a female body gender, because ~~as we all know, the other doesn't exist~~ I have one of those. In doubt, double-check paths.
{% endhint %}

1. Download the example project of files from mana's mega or Nexus and load up your Wolvenkits
2. In **Windows Explorer**, find the prepared folders per body gender:

| body gender | file path                            |
| ----------- | ------------------------------------ |
| female      | `tutorial\npv\your_female_character` |
| male        | `tutorial\npv\your_male_character`   |

3. Delete the one you're not using (do one project per NPC. No, really, I mean it.)

Now it's time to do the actual work.&#x20;

* If you want to create your V's head for Cyberpunk, read on [here](npv-preparing-the-head-in-blender.md)
* If you already have a head mesh and just want to set up the file structure, read on [here](npv-preparing-the-head-in-blender.md)

{% hint style="danger" %}
Please remember that before sharing your NPV, you **have** to change the paths! At the very least, rename the `tutorial` folders inside of `archive` and `resources` to your user name and then do a [fulltext search and replace in json](../../everything-else/moving-and-renaming-in-existing-projects.md).
{% endhint %}

##