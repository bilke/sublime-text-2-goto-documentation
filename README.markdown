# Sublime Text 2 plugin: Goto Documentation

A command to jump to documentation (on the web) for the current word. If you have [Dash](http://kapeli.com/dash/) installed you can use it instead of the web search.

## Supports

 * PHP
 * JS / CoffeeScript
 * Python
 * Clojure
 * Go
 * Smarty
 * Ruby on Rails
 * C / C++
 * Unity3D C# (TODO: currently uses standard C# scope)
 * CMake

Submit a patch adding more and I'll include it.

## Using

Open the command palette (cmd-shift-p) and choose "Goto (Dash) Documentation" while your cursor is on a word or you have some text selected.

Make a keybind by adding the following to your `User/Default (OSX).sublime-keymap`:

	{ "keys": ["ctrl+h"], "command": "goto_dash_documentation" }
	{ "keys": ["super+shift+h"], "command": "goto_documentation" } # TODO: second command does not work

(I don't like plugins automatically adding keybinds, okay.)

## Installing

First, you need to have `git` installed and in your `$PATH`. Afterwards you may need to restart Sublime Text 2 before the plugin will work.

### OSX

    $ cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/
    $ git clone git://github.com/bilke/sublime-text-2-goto-documentation.git GotoDocumentation
    $ cd GotoDocumentation
    $ git checkout dash

### Linux (Ubuntu like distros)

    $ cd ~/.config/sublime-text-2/Packages/
    $ git clone git://github.com/bilke/sublime-text-2-goto-documentation.git GotoDocumentation
    $ cd GotoDocumentation
    $ git checkout dash

### Windows 7:

    Copy the directory to: "C:\Users\<username>\AppData\Roaming\Sublime Text 2\Packages"

### Windows XP:

    Copy the directory to: "C:\Documents and Settings\<username>\Application Data\Sublime Text 2\Packages"
