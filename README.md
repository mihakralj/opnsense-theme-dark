# opnsense-theme-dark
Dark theme for OPNsense

the .txz package can be installed with:

    sudo pkg add https://github.com/mihakralj/opnsense-theme-dark/raw/main/os-theme-dark-devel-0.1.txz

after installation, a new dark theme should appear in System-General -> Theme

Default color scheme in the package is **VanHelsing**, but you can change it to any of supplied seven themes:

    cd /usr/local/opnsense/www/themes/dark/build/css
    sudo cp DraculaPro.css colors.css

after changing the color scheme, force-reload the page in the browser **(Shift-F5)**

#Seven color schemes:

DarkOrange
Blade
Buffy
Lincoln
Morbius
DraculaPro
VanHelsing
