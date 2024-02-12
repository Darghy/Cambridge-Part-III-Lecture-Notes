# How to setup my workflow

1. Install VSCode version 1.85 from November 2023. (The January 2024 update breaks tabstops when expanding snippets inside other snippets).

2. Install a TeX distribution -- I use MiKTeX, but anything should work. This will probably take a while to install.

3. Install the HyperSnips and LaTeX Workshop extensions. For HyperSnips, install version 0.2.8. To do this, install the newest version, then click on the dropdown menu next to "Uninstall" and select "Install Another Version"
(I do this because version 0.2.9 makes my snippets disappear - I think it's because the folder you want to keep them in changed for some reason - there's a workaround by manually moving them to the new folder (see Github -> HyperSnips -> Issues for more details), but easier to just use 0.2.8).

4. Open settings (Ctrl + ,), then hover the "Open Settings (JSON)" button and open the settings.json file. Add the following to the file:

        "editor.quickSuggestions": {
                "other": false,
            },


This will change the tab key's default behavior from autocompleting to jumping to the next location in our snippets.

5. Press Ctrl + Shift + P, type in "HyperSnips", open the snippet file and add your desired snippets. 

6. Sometimes the setup breaks and snippets that should only autoexpand inside a math environment start expanding everywhere. My workaround for this is to simply reload the VSCode window by pressing Ctrl + Shift + P for the Command Palette and typing in "reload" to reload the window.