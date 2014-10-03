![logo][logo]

Gotham is a **very dark** colorscheme. It was built for vim ([link][vim-gotham]
to vim colorscheme), but this repository contains versions of the colorscheme
tailored for a bunch of other platforms.

## Installation

If you use GUI vim (MacVim or gVim), [vim-gotham][vim-gotham] is the vim version
of the Gotham colorscheme. Details and installation instructions for vim are
available in the vim-gotham repository.

If you use terminal vim, check if your terminal emulator is listed in one of the
following ones. If it is, follow the instructions to install the colorscheme for
the terminal emulator; if it's not there, you can use the **256 colors version**
of the colorscheme but it doesn't look as polished as the regular one.
Instructions are available at the [vim-gotham][vim-gotham] repository.

You're more than welcome to add support for more platforms. Send me a PR!

### iTerm 2

[Download][zipped] the repository, unzip it and double-click on the
`iterm2/Gotham.itermcolors` file. iTerm will confirm the colorscheme has been
installed.

**Note** if you're on iTerm ~2.0 (stable), do the same thing but with the
`iterm2/Gotham-stable.itermcolors` file.

Now go into `Preferences > Profiles > Colors` and select `Gotham` (or
`Gotham-stable`) from the `Color Presets...` menu.

If double-clicking doesn't work, you can go to `Preferences > Profiles > Colors`
and select `Import...` from the `Color Presets...` menu. From there, select the
theme file (`.itermcolors`) and it will be imported. Now set the colorscheme to
`Gotham` (or `Gotham-stable`).

### Terminal.app

Download [terminal.app/Gotham.terminal](terminal.app/Gotham.terminal). Go into
`Terminal.app > Preferences > Profiles` and on the bottom left of the window,
click the little gear icon and click `Import...`; now select the file you
downloaded. If you want to set the colorscheme as the default one, click the
`Default` button on the right of the gear icon.

**Note** this has been tested with OSX >= 10.9 only, but let me know if it works
with previous versions too (just open an issue), thanks!

### Xresources

Copy the contents of [xresources/gotham](xresources/gotham) into your
`~/.Xresources` config file.

Then run `xrdb ~/.Xresources` to reload the config file and load the gotham
colors.

For more details about configuring Xresources see the [Arch Linux wiki
page][xresources-arch-wiki].

### PuTTY

Download [putty/gotham.reg](putty/gotham.reg).

Double-clicking on it should ask for confirmation that you want to modify the
registry.

Start PuTTY, select "Gotham" from the "Saved Sessions" list and then click
"Load" to load the colors.

### Termite

Copy the contents of [termite/gotham](termite/gotham) to your Termite
configuration file.

``` bash
mkdir -p ~/.config/termite
cd gotham-contrib
cat termite/gotham >> ~/.config/termite/config
```

If Termite is running, do <kbd>CTRL</kbd> + <kbd>SHIFT</kbd> + <kbd>R</kbd> to
reload the config file.


## Contributing

I'm more than happy to accept Pull Requests of any kind: bug fixes, support for
other editors/terminal emulators, suggestions.  If something is wrong, you can
help even by just opening an issue.

When you make a PR with support for a new platform (terminal emulator, editor,
whatever) attach a screenshot of the colorscheme in the new platform so it's
easier for me to merge right away!

**Note** if you want to tweak the colors and open a PR, make sure to open in
**in [vim's repository][vim-gotham]** and not here. Attach before and after
screenshots!


## License

MIT &copy; 2014 Andrea Leopardi, see [the license][license-file].


[logo]: http://i.imgur.com/FDLEzHC.png "Logo"
[screenshot]: http://i.imgur.com/gaGhjqh.png "An iTerm-only screenshot"
[license-file]: LICENSE.txt
[zipped]: https://github.com/whatyouhide/iterm2-gotham/archive/master.zip
[vim-gotham]: https://github.com/whatyouhide/vim-gotham
[iterm2]: http://iterm2.com/
[xresources-arch-wiki]: https://wiki.archlinux.org/index.php/Xresources
