# Sublime Text dired

A Sublime Text 3 plugin that displays a directory in a view, allowing easy file manipulation,
loosely copied from emacs dired mode.

## Installation

You can install via [Sublime Package Control](http://wbond.net/sublime_packages/package_control)  
Or you can clone this repo into your *Sublime Text 3/Packages*

## Using

The plugin provides a `dired` command which allows you to choose a directory to display.  The
files in the directory are displayed in a list allowing them to be moved, renamed, or deleted.

### Key Bindings

There is no default binding for the dired command itself, but once in a dired view the
following are available:

* `D` - delete marked files
* `M` - move marked or selected files
* `R` - rename marked or selected files
* `r` - refresh
* `m` - mark file
* `u` - unmark file
* `U` - unmark all files
* `t` - toggle all marks
* `*.` - mark by file extension

### Delete

Deletes marked files after confirmation.

### Move

The move command asks for a target directory and moves marked or selected files.

If no files are marked, all files that are part of a selection or have a cursor are moved,
allowing you to use the mark commands, multiple cursors, or selection.

### Rename

The rename command makes the view editable so files can be renamed using all of your
Sublime Text tools: multiple cursors, search and replace, etc.

To commit your changes, use `Ctrl+Enter` (dired_rename_commit).  To cancel changes, use
`Ctrl+Escape` (dired_rename_cancel).

Rename compares the names before and after editing, so you must not add or remove lines.
