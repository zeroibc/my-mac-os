# Keyboard Maestro Macros I use
## Contents
- [Explanation](#explanation)
- [KM Plugins](#km-plugins)
- [Macros](#macros)
	- [Global Macros](#global-macros)

## Explanation
One of my favourite applications that I use to significantly ease my time using my mac is [Keyboard Maestro](https://www.keyboardmaestro.com/main/) and I describe how I use it in more detail in [my wiki](https://wiki.nikitavoloboev.xyz/macOS/apps/km/km.html).

It's a wonderful tool that allows you to create very powerful macros that can range from simply pasting some text, to moving the mouse pointer to some location, to doing various calculations with the input you provide and lot lot more.

I wrote about how I manage my huge macro library [here](https://forum.keyboardmaestro.com/t/notation-i-use-to-manage-my-macros/8907).

All the macros/palettes are attached to this GitHub repository sorted into appropriate folders and I describe some of these macros/palettes below. For others, you can simply clone [this repo](https://github.com/nikitavoloboev/my-mac-os), import things and see what you like. I will be uploading essentially all the macros I use here.

All global macros will have no trigger as they are called with Applescript from [Karabiner](https://wiki.nikitavoloboev.xyz/macOS/apps/karabiner/Karabiner.html). Some macros will have a Usage comment in the beginning where I clarify how I personally use the macro. It looks like this:

<img src="https://i.imgur.com/5U1wnqz.png" width="500" alt="img">

A lot of these macros were made with great help from the [Keyboard Maestro forum community](https://forum.keyboardmaestro.com/latest).

Just to emphasize how much KM has impacted my life. My most used macro from all thse macros I share is macro to open Safari browser which I've ran [some 117,091 times](https://i.imgur.com/09KfToP.png) since I made it.

I also really love using [Alfred Maestro](https://github.com/iansinnott/alfred-maestro) workflow that lets me search through my entire KM library of actions to activate.

## KM Plugins
I really like using these KM plugins and additions. It is advised you install them as they really make using KM editor more pleasant.
- [KMFAM - Favourite actions and macros](https://forum.keyboardmaestro.com/t/macro-kmfam-favorite-actions-and-macros/4854) - This plugin lets you save complex and non complex actions and allow you to search over these actions you add quickly.

## Macros
Macros are little `KM scripts` that contain a series of actions. The macros can then be executed from a trigger, usually a hotkey.

In my case all the global macros I share (macros that can run no matter what application is currently active) have no trigger. This is because I can call these macros from Karabiner using this Applescript code:

```applescript
tell application "Keyboard Maestro Engine"
do script "g: Kill All Macros"
end tell
```

Where `g: Kill All Macros` is a macro name. Where `g:` is a prefix that stands for `global`.

Non global macros that are binded to an app will have a hotkey however. One thing to note is that the hotkey triggers are chosen with respect to my custom keyboard layout.

I have binded my control key to A key with [Karabiner](https://wiki.nikitavoloboev.xyz/macOS/apps/karabiner/Karabiner.html). My command key is E key and Command + Shift modifier is Q key. So pressing `E` key, holding it and after pressig `F` will trigger `⌘ + F` hotkey. Therefore some bindings will only make sense in context of my own layout. For example `⌃ + W` is easier to reach for me then `⌘ + D`. Because `a + w` is nicer to press then `e + d` on my keyboard. [Karabiner](https://wiki.nikitavoloboev.xyz/macOS/apps/karabiner/Karabiner.html) is one powerful abstraction that makes managing 1000+ macros easy.

### Global Macros
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