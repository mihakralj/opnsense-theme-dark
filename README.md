# opnsense-theme-dark
Dark theme for OPNsense, because real networking people dwell in the dark.

the .txz package can be installed with:

    sudo pkg add https://github.com/mihakralj/opnsense-theme-dark/raw/main/os-theme-dark-devel-0.1.txz

after installation, a new dark theme should appear in System-General -> Theme

Default color scheme in the package is **VanHelsing**, but you can change it to any of supplied seven themes:

    cd /usr/local/opnsense/www/themes/dark/build/css
    sudo cp DraculaPro.css colors.css

after changing the color scheme, force-reload the page in the browser **(Shift-F5)**

if you want to get rid of the package:

    sudo pkg delete -y os-theme-dark-devel

#Seven provided color schemes:

- DarkOrange (install with `sudo cp DarkOrange.css colors.css`)
- Blade (install with `sudo cp Blade.css colors.css`)
- Buffy (install with `sudo cp Buffy.css colors.css`)
- Lincoln (install with `sudo cp Lincoln.css colors.css`)
- Morbius (install with `sudo cp Morbius.css colors.css`)
- DraculaPro (install with `sudo cp DraculaPro.css colors.css`)
- VanHelsing (install with `sudo cp VanHelsing.css colors.css`)

Except the first one, all other color themes are inspired by Zeno Rocha's Dracula dark theme https://draculatheme.com/

You can build your own too - just peek into the **color.css** and make your own color combo! And post your color combination here as an issue!

## Problems? Glitches?

I didn't clean-up the **main.css** completely; there are plenty of direct color references still in the file (instead of using css variables) and I have no idea in which dialogs they appear. So, if something renders wrong, make a screenshot and submit an issue - or (even better) find a problematic styling block in main.css and let me know what to fix and clean.
