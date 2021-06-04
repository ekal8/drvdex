# [Code @ ParveenBhadooOfficial/Google-Drive-Index](https://github.com/ParveenBhadooOfficial/Google-Drive-Index)
Decided to start new since cloning the whole repository gets me emails from GitHub about Page Build Warnings, even disabling and removing the stuffs. Code is based on v2.0.18-beta.1

## Code Modified for Personal Use
Nothing Fancy. Name from DRiVe inDEX. Do not start here if you are making one. Instead, go here:
https://github.com/ParveenBhadooOfficial/Google-Drive-Index

## Sources and Credits
I have read the code and the sources, especially the licenses involved, and this repository is abiding by the licenses and intellectual property.
There is absolutely no reason a copyright notice or license violation letter will arrive on my doorstep.

* https://github.com/ParveenBhadooOfficial/Google-Drive-Index
* https://bootswatch.com/
* https://fonts.google.com/icons
* https://github.com/dharmatype/Bebas
* https://css-tricks.com/emojis-as-favicons/
* https://freefrontend.com/html-css-404-page-templates/ > https://codepen.io/igloude/pen/qNNWKr
* Favicon and Folder Icon idea from Spencer Woo.
* Emoji stored in your device, if it had one.
* Big thanks to https://stackedit.io for helping me make this file

# Yea i know, but, can "You" use it for your needs too?
Yea, this is just a custom dark theme. Read the code first, especially app.js and worker-beta.js before using it. Do note that I removed the drive selector thing, but you can use multiple drives by changing the link such as `https://a.demo.workers.dev/0:/` to `https://a.demo.workers.dev/1:/`.

Want to get your hands dirty and modify the entire site? Clone/Fork [The Repository](https://github.com/ParveenBhadooOfficial/Google-Drive-Index), or this Repository (clone only pls), if that is your liking and wanna depend on no one.

##  One More Thing. Please Read if you really in to it.
**Don't ask or bother** the ones who made the code and also me about this thing or my entire repository about anything you can ask for, they *might* **not help you** and so am I. You're on your own to figure out your own issues.

Also, equip your best eyes and brain on this work. You have been reminded.

## Using this theme
Before starting, You must generate your worker-beta.js file. Or, have a working worker-beta.js file and edit just a few lines.

**Don't have a working worker-beta.js file?**
> Go modify [worker-generator.js](https://github.com/ParveenBhadooOfficial/Google-Drive-Index/blob/master/worker/worker-generator.js), copy paste code to workers, change up the Client ID and Secret to generate your own creds, deploy on workers to get the Refresh Token, copy the generated one, create another worker, paste the code on the new worker, and you're done. 

> Or, you can just go to https://gdi.js.org and follow the conventional and easy way. **Recommended** if you're new to this stuff.

## To apply this theme:
1.  Add this line `"footnote": "the footnotes",`  under `const uiConfig = {`  as you won't be needing the lines `"copyright_year": "", "company_name": "", 
"company_link": ""`.  Change the value of footnote to your words. (Reason for this, is if you want something other than or more than a copyright signature).

> There are other lines you won't be needing, such as the `"contact_link": "",` and others. You'll realize it after deploying.

2. Change `"jsdelivr_cdn_src"` value and add in `"https://cdn.jsdelivr.net/gh/lsn00/drvdex"` (or your own repo if you have your own)
3.   Change lines `"theme": "",` and `
"version": ""` to `"theme": "darkly",` and `
"version": "#"` where the # is the version number.

### Version Number (only for this theme). More details [here](https://github.com/lsn00/drvdex/releases).
v1
>-   Switched some SVGs to Emojis.
>- Removed Drive Selector
>-   Changed words on result page.
>-   Removed most navigation bar stuff.
>-   Removed the hyperlink on the footer, this requires changing the workers code to use the footer.
>-   Copy Button and the long URL bar is nowhere to be seen, front-end.
>-   Removed some subtitle options for plyr.
>-   Removed gradient from the audio player.
>-   Removed features of the Encoded JSON.

v2
>- All stuffs in Previous Version
>- Resurrected the URL/DDL Link, copy button yeeted tho and will not come back.

v3
>- All stuffs in Previous Version
>- Removed the Breadcrumb thing

v4
>- All stuffs in Previous Version
>- Removed the URL/DDL Link bar

### Now back to the tutorial...
4. Find the line `<link href="https://cdn.jsdelivr.net/npm/bootswatch@5.0.0/dist/${uiConfig.theme}/bootstrap.min.css" rel="stylesheet" crossorigin="anonymous">` if you're using the original worker-beta.js or a similar name that ends in `/bootstrap.min.css`. It is under the "Do Not Edit" line.
5. Now, replace the link with `https://cdn.jsdelivr.net/gh/lsn00/drvdex/css/bootstrap/dark/bootstrap.css` or your own version.

Then, You're all done.

You can experiment stuffs in `const uiConfig` for more options.

*This is the best I can do at explaining. If you have been working on code, you can find this a bit easy. I don't answer any questions or features so, you're on your own. I'm out of braincells, but you can try to explain this in even more detail if you can by sharing your own version of this guide to others. Credit optional.*

## Fun Facts:
* `const unauthorized =`  and `const not_found =` in worker-beta.js are just html error pages, change it up if you want to.
* to make the favicon be an emoji, change value of `favicon` to `data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>🗂️</text></svg>` and change the emoji to your preferences.
* code is served by [jsDelivr](https://www.jsdelivr.com/) to handle `GET` from Github. Syntax is `https://cdn.jsdelivr.net/gh/`.
