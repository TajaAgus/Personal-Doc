# Personal-Doc

This small program is to be as a quick personal(or shared via repository) documentation access in a terminal.
I personally use it as a infra/devops tool to have quick access to my own commands, and it's super easy and friendly to use! It reuses less in the background to display and navigate the files.

## Installation

After cloning the project, you can either:
1. Add it to your personal `bin` for quick access in the terminal, or
2. Use the built-in installation command: `./doc -i` or `./doc --install`

The installation command will automatically add the script's path to your `.zshrc` file, allowing you to run `doc` from anywhere in your terminal.

## Usage

* `doc`: Displays all command files
* `doc filename`: Display contents of a specific command file
* `doc -e filename`: Edit or add a new commands file
* `doc -x filename`: Archive a commands file (moves to archived folder)
* `doc -i` or `doc --install`: Add script path to .zshrc for global access
* `doc --version`: Show version information