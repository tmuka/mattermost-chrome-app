this is a little chrome app wrapper so the open source slack clone, ["mattermost"](http://www.mattermost.com/) can be run in an isolated chrome window that opens links in the main chrome instance. Since it's a chrome app, you can pin the app icon to the windows start menu.  clicking links in chat open in Chrome, not in the chat window.

This is unofficial, not related or approved by anyone, but it is working nicely for myself and my team.  


I only tried this in Windows 7 using Chrome stable, it will probably work anywhere chrome runs, git it a try!

# Mattermost Chrome Web App
This is a chrome extension that provides a web wrapper to make mattermost chat work like a standalone chrome app so links will open in your main chrome window.
![](https://raw.githubusercontent.com/tmuka/mattermost-chrome-app/master/mattermost_chrome_app_screenshot.png)

## To set your own url and try it unpacked
1. `git clone https://github.com/tmuka/mattermost-chrome-app.git` onto your local machine
1. edit manifest.json file and update the "urls" and "web_url" lines with your mattermost team url. save changes.
1. in chrome, open url chrome://extensions/
2. enable checkmark "Developer mode" (this will let you install an unpacked local extension)
3. click "Load unpacked extension"
4. browse to and select the folder you cloned this project into.
5. that should have added an white icon for "Mattermost Chrome App", right click on it, click "App Info". change from "Open in Tab" to "Open as window", click "Create shortcuts".

## To pack the extension
1. in chrome, open url chrome://extensions/
2. enable checkmark "Developer mode" (this will let you install an unpacked local extension)
3. click "Pack extension"
4. click browse for "Extension Root Directory" and select the folder you cloned and configured
5. click "pack extension", save the file to wherever you want it for installation and sharing

## To install packed extension
1. in chrome, go to url chrome://apps
2. open windows explorer, navigate to the folder you saved mattermost_chrome_app.crx file into. drag and drop that file onto the chrome://apps window.
3. that should have added an white icon for "Mattermost Chrome App", right click on it, click "App Info". change from "Open in Tab" to "Open as window", click "Create shortcuts".

Now you should have an icon in your taskbar quick launch and start menu to directly open Mattermost chat.

## Bonus Custom CSS
I also use a few lines of custom CSS that make the view more compact. I use the [Stylish chrome extension](https://chrome.google.com/webstore/detail/stylish/fjnbnpbmkenffdnngjfgmeleoegfcffe?utm_source=chrome-app-launcher-info-dialog) to apply the styles located in the mattermost_compact.css file.

## Future enhancements
1. It uses chrome html5 notifications which work okay, but it would be nice if the taskbar icon would flash on new notifications too, maybe somebody knows how to do that in a chrome app?
