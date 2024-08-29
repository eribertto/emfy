0.4.0 (2024-08-29)
------------------

### Changed

- Reduce `emacs-init-time` by approximately 40% by delaying package
  loading until usage time.
- Use `with-eval-after-load` to delay the evaluation of expressions
  that depend on certain packages to be loaded.
- Use `setopt` instead of `setq`.
- Enable `show-trailing-whitespace` only in modes pertaining to
  configuration, programming, and text.
- Introduce `install-packages` command to install packages.
- Use `fboundp` to check if a mode exists before adding hooks that
  enable that mode.
- Prevent Paredit from altering the behaviour of `RET`.


0.3.0 (2023-06-22)
------------------

### Added

- Always add a newline automatically at the end of a file while saving.


### Changed

- Leave menu bar enabled.
- Increase contrast for isearch and lazy highlighting.


0.2.0 (2022-01-02)
------------------

### Added

- Enable `fido-mode`.
- Custom key sequence `C-c d` to delete trailing whitespace.


### Fixed

- Load custom-file.


0.1.0 (2021-12-31)
------------------

### Added

- Disable menu bar.
- Disable tool bar.
- Disable scroll bar.
- Use `wombat` theme.
- Customize faces for background, cursor, searches, and comments.
- Enable and configure `ido-mode`.
- Show trailing whitespace.
- Indicate non-existing lines in the left fringe.
- Indicate buffer boundaries in the left fringe.
- Use single spacing convention to end sentences.
- Use spaces, not tabs, for indentation.
- Enable `show-paren-mode` to highlight matching parentheses.
- Write auto-saves and backups to `~/.emacs.d/backup/`.
- Do not move the current file while creating backup.
- Disable lockfiles.
- Workaround for https://debbugs.gnu.org/34341 in GNU Emacs <= 26.3.
- Automatic installation of packages from MELPA.
- Write customizations to `~/.emacs.d/custom.el` instead of `~/.emacs`.
- Install Markdown Mode.
- Install Paredit.
- Install Rainbow Delimiters.
- Enable Paredit in Emacs Lisp mode, eval-expression minibuffer, IELM
  mode, Lisp interaction mode, and Lisp mode.
- Enable Rainbow Delimiters in Emacs Lisp mode, IELM mode, Lisp
  interaction mode, and Lisp mode.
- Customize Rainbow Delimiters colors to show colorful parentheses.
- Custom command to show current time.
- Custom key sequence to show current time.
- Start Emacs server automatically, if it is not running already.
- Command named `em` to run Emacs server and client.
