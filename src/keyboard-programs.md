# Keyboard-Friendly Programs

Command-line interface (CLI) programs with keyboard control boost productivity because grabbing the mouse does not interrupt work.

## Keyboard-Driven Browsing

Several web browsers are designed for keyboard-driven control.

> **Hack:** Install a browser plugin for keyboard-control, such as Surfingkeys (available for Firefox and Chrome-like browsers).

However, often they present compatibility issues. Mostly, this is the responsibility of the web developers. But from an end user's perspective, one is better off with a standard browser such as Google Chrome or Firefox. Surfingkeys and similar plugins enable a vim-like control of the web browser, and the hands can remain on the keyboard.

## The Editor

For writing scientific texts, we need a suitable editor. I decided on Vim - according to the 'church of Emacs,' this is the 'editor of the beast' (look for information about the editor war on the internet).

> **Hack:** Use an editor which is usable without a mouse, such as Vim.

If you accidentally entered Emacs, you can leave it with `Ctrl+x` `Ctrl+c`.

In case you are not familiar with Vim, you should start the `vimtutor` (terminal). This command will open Vim and give you a 30-minute introduction on how to use this mighty editor.

## Markdown and Pandoc

Why Markdown:

A short introduction to Markdown/Pandoc for academic publishing is given in [@krewinkel_formatting_2017].

- Plain text files with simple syntax. It can be directly read and edited with many programs.
- There are both particular Markdown word processors ('what you see is what you mean') and generic editors.

Several editors, such as Vim and Emacs, have plugins to work with Markdown.

For example, I'm using the following Plugins in Vim:

- `vim-pandoc/vim-pandoc`
- `vim-pandoc/vim-pandoc-syntax`
- `ycm-core/YouCompleteMe`

Vim has already an integrated spellchecker for many languages.

Unfortunately, grammar checking Plugins such as 'vim-grammarous' and 'vim-LanguageTool' are too demanding for the Pi 0. Instead, we can check the grammar of the file using `gramma` or with the online service of Grammarly.

- `preservim/vim-wordy`

The handling of references is essential.

The final formatting can be done with Pandoc [@krewinkel_formatting_2017].

## PDF Viewer

`zathura`

## Email

- alot
- Notmuch
- offlineimap
- msmtpq-queue
- aerc

## Asynchronous and Offline Mailing

`offlineimap` for synchronizing remote IMAP folders with local Maildir folders.

`msmtp` for sending emails.

You can get queuing capabilities for sending mails by installing [https://gitlab.com/lxkl/msmtpq](https://gitlab.com/lxkl/msmtpq). Instead of sending emails immediately, they are added to the queue by `msmtpq-enqueue`. Calling `msmtpq-flush` will ship out all mails.

Alot integrates well with an `abook` or `khard` address book.

Additional functions can be easily programmed in Python. The alot developers and community published many code examples and are very helpful in case of questions.

For example, HTML messages can be passed to a graphical browser for rendering them correctly.

## Software List

| Software | Type | Description |
|----------|------|-------------|
| **alot** | Email | CLI-interface for Notmuch, an email database. It can work offline and requires external programs for synchronization. Handles A LOT of mail. [@totzke_alot_2022] |
| `bibman` | Citation | Uses the BibTeX format; manager compatible with LaTeX and markdown/Pandoc. |
| `cadaver` | WebDAV | File exchange with Cloud client storage such as NextCloud. |
| `kpcli` | Password | Compatible with KeePass manager databases. |
| `nsgtk3` | Web browser | Efficient graphical web browser with own renderer. |
| `ranger` | File manager | Miller columns for display of directories and files. |
| `vim` | Editor | Powerful editor; extensible by plugins; supporting most text and code styles. |
| `vimtutor` | Tutorial | Starts the Vim tutorial! |
| `xlinks2` | Web browser | Efficient CLI browser for X with image view. |
| `uzbl` | Web browser | WebKit browser with Vim key bindings and fair memory use. |
| `w3m` | Web browser | Terminal web browser with image view and vim-style keys. |
| `zathura` | PDF viewer | Uses vim-style keybindings. |

*CLI-command line interface, GUI-graphical user interface, VIM-vim-style operation.*
