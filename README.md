this is a little chrome app wrapper so the open source slack clone, ["mattermost"](http://www.mattermost.com/) can be run in an isolated chrome window that opens links in the main chrome instance.
I only tried this in Windows 7 using Chrome stable, it will probably work anywhere chrome runs, git it a try!

# Mattermost Chrome Web App
This is a chrome extension that provides a web wrapper to make mattermost chat work like a standalone chrome app so links will open in your main chrome window.
## To try it
1. in chrome, open url chrome://extensions/
2. enable checkmark "Developer mode" (this will let you install an unpacked local extension)
3. click "Load unpacked extension"
4. that should have added an white icon for "Mattermost Chrome App", right click on it, click "App Info". change from "Open in Tab" to "Open as window", click "Create shortcuts".

## To install
1. in chrome, go to url chrome://apps
2. open windows explorer, navigate to the folder you saved mattermost_chrome_app.crx file into. drag and drop that file onto the chrome://apps window.
3. that should have added an white icon for "Mattermost Chrome App", right click on it, click "App Info". change from "Open in Tab" to "Open as window", click "Create shortcuts".

Now you should have an icon in your taskbar quick launch and start menu to directly open Mattermost chat.
