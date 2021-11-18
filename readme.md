# MORROWIND#: A Morrowind Modding Guide

Last updated: November 18th, 2021

![Banner](https://raw.githubusercontent.com/Sigourn/morrowind-sharp/master/Main%20Banner.jpg)

## Contact info

You can find me in the [Morrowind Modding Community](https://discord.me/mwmods) Discord, in addition to the following sites.

- Nexus Mods: [Lucas9](https://www.nexusmods.com/morrowind/users/14600469)
- Reddit: [Sigourn](https://www.reddit.com/user/Sigourn)
- RPG Codex: [Sigourn](https://rpgcodex.net/forums/index.php?members/sigourn.21476/)

## Acknowledgments

I want to thank the following people for their support. Not only for their kind comments towards me and the guide, but also for having gone the extra length and financially supporting me!

- **Tythesly** (August 11th, 2021)
- **JFS** (August 24th, 2021)

## About

> To play Morrowind# is to play Morrowind the way *I* want to play it.

What *is* Morrowind#?

A modular modding guide for The Elder Scrolls III: Morrowind. It's been in the works for a handful of years already, when I first decided I wanted to keep a track of what mods I liked to play with, and how to install the most problematic of them.

Over time, I realized I wanted to share my setup with others. This in turn lead to me expanding the guide to account for more detailed instructions, in hopes that those less familiar with the game and modding in general wouldn't have such hard times setting up the mods that make up this guide.

Because I like to think of myself as someone organized, the guide is split in two parts:

- [**Setup**](https://github.com/Sigourn/morrowind-sharp/blob/master/setup.md#morrowind-setup), where I walk you through to getting the necessary patches, tools and utilities, as well as our mod manager up and running.
- [**Morrowind#**](https://github.com/Sigourn/morrowind-sharp/blob/master/mw%23.md#morrowind), which is the bulk of the guide, and where we will be installing our mods proper.

Why is this the case? Because **Setup** should be useful to anyone looking to play Morrowind, hence why I don't consider it to be part of **Morrowind#**, which is what makes this guide *mine* as opposed to someone else's. In essence, to play Morrowind# is to play Morrowind the way *I* want to play it.

However, Morrowind# is not for everyone. I split the guide into a number of standard modules, mostly for organization, but also because it helps keep compatibility issues in check (mods that alter the user interface are more likely to conflict with mods that alter the user interface; mods that modify visuals are more likely to conflict with mods that modify visuals, etc.).

On top of that, each module has a selection of E for Everyone mods. These are just great mods that make Morrowind that much more enjoyable in 2021, without demanding a considerable amount of time to setup them up compared to, say, if you wanted to install the entirety of the mods present in Morrowind# (*a lot* for the average Joe, not that many for modding enthusiasts).

I like to mod my games with the following in mind:

- I don't want crashes.
- I don't want bugs.
- I want my mods to blend in, be them gameplay, audio, or visual mods. The last thing I want is for a mod to stick out like a sore thumb.
- I want my mods to be compatible with each other.
- I want my setup to be compatible with other mods, for the most part.

Because of this, the are a handful of mods you won't see in this guide:

- Big overhauls, be them towns, quests, or gameplay overhauls.
- Visual mods along the lines of texture and mesh replacers. Morrowind is an old game, and I find the best way to make it look good is to slap MGE XE and shaders on top, as well as a selection of tasteful visual mods that enhance what's already there. These mods tend to make up the bulk of most modding guides for any given Bethesda game. Here, not so much.
- Mods that add new equipment. Integration into the base game is everything, so I chose to leave these out just to avoid headaches.

What I offer you is my idea of Morrowind. All I ask in return is your patience when it comes to following instructions. If I took the time to write them, you can take the time to read them.

## Frequently asked questions

### Is this guide compatible with OpenMW?

No. Many mods in this guide rely on the Morrowind Script Extender (MWSE), which is incompatible with OpenMW. That said, many individual mods will be compatible. But I can't point these out for you.

### Is this guide compatible with Morrowind Rebirth?

No. This guide changes many aspects of the game which will be incompatible with Morrowind Rebirth. That said, many individual mods will be compatible. But I can't point these out for you.

### Is this guide compatible with Tamriel Rebuilt?

Though compatibility with Tamriel Rebuilt itself is very good, Tamriel Rebuilt content will not benefit from the improvements made by many of the mods suggested here, such as visual or gameplay improvements.

### Is this guide compatible with (mod)?

I can't say for sure. I can only give an opinion, but at the end of the day there's no substitute for reading the description of the mod and checking for compatibility in TES3View. Same goes for questions regarding mod order and load order. The less mods you install from the guide, the better the chances any mod you install will be compatible with it.

### How many plugins and mods are there?

I tried to keep the amount of recommended mods relatively short and to the point. Most guides include a *huge* amount of graphic mods (retextures and mesh improvements), whereas I prefer to focus on specific graphical tweaks or visual effects that add to the game instead of changing what's already there.

There are roughly 130 recommended (a.k.a. "essential") mods, totalling about 30 plugins. For people who love to mod their games, there are roughly 240 mods and about 70 plugins.

### How much space do I need to install these mods?

Roughly 23GB, of which **Intelligent Textures**, **AURA**, and **TUBES4MUSE** account the majority of. However, only the former is strongly encouraged that you install if this is your first time playing Morrowind.

### How much time will it take me to install all mods?

Depends on how quick and thorough you are about it. I guarantee it will take you far less time than to set up most other Morrowind guides, bar the most spartan ones.

### How often is the guide updated?

*Very* often. Those who have been followed this guide's progress for a good while already know that mods can (and *will*) be removed if my opinion changes about them. Likewise, they can be added back if I feel they added an extra to the game it's hard to play without.

### Is there a Wabbajack installer for the guide available?

No. On top of the additional amount of work, I don't want an installer that automates this guide's installation. People are free to make one if they wish, but I'm against anything that allows people to install hundreds of mods in one go without even knowing what they are installing. People failing to read the instructions and descriptions placed in the guide account for a good 90% of the problems they report. This is not a behavior I want to encourage with a Wabbajack installer.

### Do you have a Patreon?

Believe it or not, I've been asked this enough times for me to make it a FAQ. The truth is I don't want to be put in a position where I feel obligated to answer to others. The moment I don't feel like maintaining my guide anymore is the moment where quality will start to drop if I keep updating it out of an obligation to others. Neither you nor me want that to happen. That you enjoy this guide is all I need.

However, if you *feel* like I deserve some compensation for this guide, I'm always open to be given a game as a gift from my [GOG Wishlist](https://www.gog.com/u/Lucas9/wishlist)! Sadly, we (Argentina) are charged a hefty extra for spending money on foreign products, which means buying games is far more expensive than it should be (about 60% more expensive). If you buy me a game, I'll add your name to the guide for everyone to see.

## My setup

When installing all mods in this guide, as well as the recommended shaders, my framerate ranges anywhere from 10fps (at worst, in the Grazelands) to 30fps (indoors), through 20fps outdoors. For reference, here is a my setup.

System | My Specs
------------ | -------------
Operative System | Windows 8.1 Pro 64-bit
CPU | Intel Core i5 4440
RAM | 8GB
Graphics | 1GB ATI AMD Radeon HD 7700 Series
HDD | 1TB
Monitor | Samsung 24" 1080p @ 60Hz
