# vnotes

Manage your notes with flat files and your system text editor

## Dependencies

* [bash](https://www.gnu.org/software/bash/bash.html)
* [coreutils](https://www.gnu.org/software/coreutils/)
* [kbd](http://www.kbd-project.org)
* [ncurses](https://invisible-island.net/ncurses/ncurses.html)

## Configuration

Configuration is handled using environment variables:

* `EDITOR`: The text editor that should be used to open notes (default: `/usr/bin/vim`)
* `VNOTES_FOLDER`: The folder notes should be managed in (default: `$HOME/Notes`)
* `VNOTES_EXTENSION`: The file extension notes should have (default: `md`)

## Usage

* `vnotes [PATTERN]`: If multiple notes include `[PATTERN]` a list of matching notes is presented to choose from, otherwise it opens the closest matching note
* `vnotes -c|--create [NAME]`: Creates a new note named `[NAME]`
* `vnotes -d|--delete [NAME]`: Deletes the note named `[NAME]`
* `vnotes -h|--help`: Shows the help text
