# GoVim - Simple Vim Clone in Go

GoVim is a small clone of the Vim text editor implemented in the Go programming
language using the tcell package. The primary objective of this project is to
learn and practice design patterns by incorporating concepts from various
design patterns books and online resources. The focus of GoVim is to implement
core functionalities displayed in the Vim tutor, allowing users to manipulate
text efficiently.

## Features

GoVim aims to provide the following core features:

1. **Basic Text Editing**: Users can create, open, edit, and save plain text
   files. The editor will support common text manipulation commands like
   insert, delete, and change.

2. **Cursor Movement**: The editor allows users to navigate the text using
   standard Vim navigation commands, such as h, j, k, l, and word-wise
   movements.

3. **Undo/Redo**: Users can undo and redo their actions, allowing them to
   revert changes and navigate editing history.

4. **Search and Replace**: GoVim will enable users to search for specific text
   patterns and perform replacements as needed.

5. **Copy, Cut, and Paste**: Users can copy, cut, and paste text selections,
   enhancing editing capabilities.

6. **Modes**: The editor will implement different modes for navigation and
   editing, including normal mode, insert mode, and command mode, similar to
   Vim.

7. **Syntax Highlighting** (Optional): If time permits, GoVim may include
   syntax highlighting for specific programming languages or file types.

## Installation

To run GoVim, you need to have Go installed on your machine. If you don't have
it yet, you can download and install it from the official Go website:
https://golang.org/dl/

Once Go is set up, you can clone the GoVim repository to your local machine
using the following command:

```
git clone https://github.com/your-username/govim.git
```

## Dependencies

GoVim utilizes the `tcell` package to handle terminal input and output. You can
install it using the following `go get` command:

```
go get github.com/gdamore/tcell/v2
```

## Usage

To run GoVim, navigate to the project's root directory and execute the
following command:

```
go run main.go
```

Once the editor starts, you can use the following commands:

- **i**: Enter insert mode (to start editing).
- **Esc**: Return to normal mode (from insert mode or other modes).
- **hjkl keys**: Navigate the text in normal mode.
- **:w**: Save changes (in normal mode).
- **:q**: Quit the editor (in normal mode).
- **:wq**: Save and quit (in normal mode).

Remember, GoVim is a small project aimed at learning and practicing design
patterns, so it may not have the full feature set of Vim. However, it should
provide a basic understanding of how a text editor like Vim works.

## Design Patterns

GoVim incorporates design patterns inspired by various design patterns books
and online resources. Some design patterns you may encounter in the codebase
include:

- Command Pattern: Used to encapsulate various operations as commands, which
  can be invoked, queued, and undone.

- Memento Pattern: Employed to implement undo and redo functionality by saving
  and restoring the editor's state.

- Iterator Pattern: Used for traversing and manipulating text content
  efficiently.

- Observer Pattern: Possibly employed to update the user interface when changes
  occur in the editor.

## Contributions

GoVim is primarily a personal learning project. However, if you find any bugs,
issues, or have suggestions for improvements, feel free to open an issue or
submit a pull request. Contributions and feedback are always welcome!

## License

GoVim is distributed under the [MIT License](LICENSE), making it open-source
and free to use.

## Acknowledgments

This project wouldn't have been possible without the valuable resources and
knowledge shared by the open-source community and authors of design patterns
books and online tutorials.

