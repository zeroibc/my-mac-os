# Keyboard Maestro Macros I use
One of my favourite applications that I use to significantly ease my time using my mac is [Keyboard Maestro](https://www.keyboardmaestro.com/main/) and I describe how I use it in more detail in [my wiki](https://wiki.nikitavoloboev.xyz/macOS/apps/km/km.html).

It's a wonderful tool that allows you to create very powerful macros that can range from simply pasting some text, to moving the mouse pointer to some location, to doing various calculations with the input you provide and lot lot more.

I wrote about how I manage my huge macro library [here](https://forum.keyboardmaestro.com/t/notation-i-use-to-manage-my-macros/8907).

All the macros/palettes are attached to this GitHub repository sorted into appropriate folders and I describe some of these macros/palettes below. For others, you can simply clone this repo, import things and see what you like. I will be uploading essentially all the macros I use here.

Most macros will have a Usage comment in the begenning where I clarify how I personally use the macro. It looks like this:

<img src="https://i.imgur.com/5U1wnqz.png" width="500" alt="img">

A lot of these macros were made with great help from the [Keboard Maestro forum community](https://forum.keyboardmaestro.com/latest).

## Contents
- [Global Macros](#global-macros)

## Global Macros
Glocal macros can be found [here](macros/global).


- Open and filter websites in safari (credit to [Christopher Stone](https://github.com/ccstone))
	- One of my most used macros that when activated will open a website that is specified inside `urlToFetch` field.
	- And it will match all current tabs with name specified in `urlFilterText` field.
	- This specific macro will open [hckr news](https://hckrnews.com/) and will jump between [news ycombinator open tabs](https://news.ycombinator.com/).
	- I use it heavily throughout the day.
	- The example macro I provide is for Hacker News.
		- You can change it to the website you like.

<img src="https://i.imgur.com/fAVRcl8.png" width="500" alt="img">

- Open and filter websites in chrome (credit to [Christopher Stone](https://github.com/ccstone)).
	- Same principle as above but for chrome.
	- Example macro opens localhost:3000 but you can change it to what you like.

## Safari Macros
- Open current url in chrome
	- Will open your current Safari URL in chrome.
	- I often use it if I need to use dev tools on the site or if the site has flash content.
- Safari main actions
	- One of my most used macros in Safari.
	- Essentially the trick is that I can set my own site specific hotkeys by using a switch statement on current safari URL content.
	- This macro for example, when I have a google page with results open, if run, will select the first result instantly.
	- If I am on duckduckgo page, this same macro will select the first duckduckgo result.
	- These are just few examples of what you can do.
		- Essentially you can create your own little actions for any of the websites you visit if you wish (I use ⌃ + e,r,v,b,n,m for site specific hotkeys).

## KM Palettes
I also really love [KM Palettes](https://wiki.keyboardmaestro.com/manual/Palettes) feature and use that a lot. Here are some of the Palettes I have made that you can download and use.

## Macro Sets for apps
Aside from these specific useful macros I link above as well as the palettes. You can also find entire macro sets for apps that I use [here](/macros/macro-sets).

## App Specific Palettes
App Specific palettes can be found and downloaded from [here](/palettes/app).