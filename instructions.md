# How to setup my workflow

1. Install VSCode version 1.85 from November 2023. (The January 2024 update breaks tabstops when expanding snippets inside other snippets).

2. Install a TeX distribution -- I use MiKTeX, but anything should work. This will probably take a while to install.

3. Install the HyperSnips and LaTeX Workshop extensions. For HyperSnips, install version 0.2.8 (version 0.2.9 breaks things).

4. Open settings (Ctrl + ,), then hover the "Open Settings (JSON)" button and open the settings.json file. Add the following to the file:

        "editor.quickSuggestions": {
                "other": false,
            },


This will change the tab key's default behavior from autocompleting to jumping to the next location.

5. Press Ctrl + Shift + P, type in "HyperSnips", open the snippet file and add your desired snippets. 