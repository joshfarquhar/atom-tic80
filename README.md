# atom-tic80

<big>Make and run [TIC-80](https://tic80.com/) games in [Atom](https://atom.io/)</big>

----

<!-- This package for [Atom Editor](https://atom.io/) adds functionality to easily edit and run [TIC-80](https://tic80.com/) games. -->

<!-- This customizable package for [Atom Editor](https://atom.io/) allows you to make and run [TIC-80](https://tic80.com/) games and print all the console output to a built-in terminal. -->

* Allows you to run and make games within Atom
* Prints TIC's console output in Atom's terminal
* Provides autocomplete and snippets for TIC's API

![Showcase](https://user-images.githubusercontent.com/51688199/91285388-96dee980-e7a6-11ea-840f-44fee158a08a.gif)

## Installation

Either run command:<br/>
* `apm install atom-tic80`

Or:
1. Go to Atom > Settings > Install
2. Search for `atom-tic80`
3. Click "Install"

## Usage

All commands can be ran via [Command Palette](https://flight-manual.atom.io/getting-started/sections/atom-basics/#command-palette). If you open it by pressing `Ctrl+Shift+P` and type `tic80`, you will see all the available commands.

### Run

`Tic80: Run` command simply runs TIC-80. Although, it's not that simple because Atom needs to know how to run do it.

Try out the command: if it fails, go to the package settings and set proper path to your TIC-80 executable file.

### Run file

##### Basics

Using `Tic80: Run File` you can make your games right in Atom! Write some code, save it as .lua (or .js or whatever TIC-80 supports) and press `Ctrl+R` (the command has a handy keybinding!).

The same command can also run .tic files. However, it's not recommended to edit them using Atom (or any other external text editor) because chances are this action will corrupt the files.

##### Game assets

Sprites, tiles, music and other game assets, should be stored in a separate file with .tic extension that should be named the same way and moved into the same directory as your code file (e.g. `dir/game.lua` and `dir/game.tic`).

However, it's possible to have everything in one file ([read](#all-in-one-file)).

### Project

##### How to make one

As an additional feature, with `Tic80: Create Project` you can create cart and code files in a preferred folder and start making games straight away!

1. Run `Tic80: Create Project` command
2. Choose folder
3. Wait for TIC-80 to open
4. *(optional)* Run `new [language]` if you want to use a language different from Lua (e.g. `new js`)
5. Run `save <your-game>`
6. ...
7. Done!

##### All-in-one file

Since 0.80.0, using TIC's PRO-version, you can save cart files as code files. If you want to keep both code and game assets in a single file, specify extension in step 5 (e.g. `save <your-game>.lua`).

<!-- screenshot -->

### Terminal

The package can print TIC-80 console output to a terminal within Atom. You can tweak its behavior and properties in the package settings.

![Terminal](https://user-images.githubusercontent.com/51688199/91285403-9b0b0700-e7a6-11ea-9533-67eecaf708c2.png)


### Autocomplete and snippets

The package also includes autocomplete feature for TIC's API and some handy snippets.

![Autocomplete](https://user-images.githubusercontent.com/51688199/91285376-95152600-e7a6-11ea-930d-e2aabddad208.png)

## Changelog

Changelog can be found in the [CHANGELOG](CHANGELOG.md) file.

## License

This project is licensed under the terms of MIT license, See the [LICENSE](LICENSE.md) file for more info.
