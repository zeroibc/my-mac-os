# Keyboard Maestro Macros I use 
One of my favourite applications that I use to significantly ease my time using my mac is [Keyboard Maestro](https://www.keyboardmaestro.com/main/) and I describe how I use it in more detail in [my wiki](https://nikitavoloboev.gitbooks.io/knowledge/content/macOS/apps/km/km.html).

It's a wonderful tool that allows you to create very powerful macros that can range from simply pasting some text, to moving the mouse pointer to some location, to doing various calculations with the input you provide and lot lot more.

All the macros / palettes are attached to this GitHub repository sorted into appropriate folders and I describe some of these macros / palettes below. For others, you can simply clone this repo and see what you like. I will be uploading essentially all the macros I use here.

## Global Macros 
- Get current url from safari
	- will get the URL of your current tab and put it into your clipboard
	- I reuse this macro quite often in other macros too where I need to do things with the URL (either modify it or pass it somewhere)
- Clone repo to ~/play
	- I wrote about how I use this macro [here](https://medium.com/@NikitaVoloboev/insta-cloning-ff5f38eb1d32)
	- essentially if you are looking at some repo on GitHub, running the macro will clone it to a folder you specify (I use ~/play)
- Open and filter websites in safari
	- one of my most used macros that when activated will open a website that is specified inside `urlToFetch` field
	- and it will match all current tabs with name specified in `urlFilterText` field
	- this specific macro will open [hckr news](https://hckrnews.com/) and will jump between [news ycombinator open tabs](https://news.ycombinator.com/)
	- I use it heavily throughout the day
	- the example macro I provide is for hacker news
		- you can change it to the website you like

<img src="https://i.imgur.com/fAVRcl8.png" width="500" alt="img">

- open and filter websites in chrome
	- same principle as above but for chrome
	- example macro opens localhost:3000 but you can change it to what you like

## Safari Macros 
- open current url in chrome
	- will open your current Safari URL in chrome
	- I often use it if I need to use dev tools on the site or if the site has flash content
- safari main actions
	- one of my most used macros in Safari
	- essentially the trick is that I can set my own site specific hotkeys by using a switch statement on current safari URL content
	- this macro for example, when I have a google page with results open, if run, will select the first result instantly
	- if I am on duckduckgo page, this same macro will select the first duckduckgo result
	- these are just few examples of what you can do
		- essentially you can create your own little actions for any of the websites you visit if you wish (I use ⌃ + e,r,v,b,n,m for site specific hotkeys)

## KM Palettes 
I also really love [KM Palettes](https://wiki.keyboardmaestro.com/manual/Palettes) feature and use that a lot. Here are some of the Palettes I have made that you can download and use.

## App Specific Palettes 
App Specific palettes can be found and downloaded from [here](/palettes/app). They include :

- Alfred Preferences
- Safari

## Macro Sets for apps
Aside from these specific useful macros I link above as well as the palettes. You can also find entire macro sets for apps that I use [here](/macros/macro-sets). Currently it has sets for : 
- Alfred Preferences