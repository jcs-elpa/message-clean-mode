[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![JCS-ELPA](https://raw.githubusercontent.com/jcs-emacs/jcs-elpa/master/badges/v/message-clean-mode.svg)](https://jcs-emacs.github.io/jcs-elpa/#/message-clean-mode)

# message-clean-mode
> Keep messages buffer clean

[![CI](https://github.com/jcs-elpa/message-clean-mode/actions/workflows/test.yml/badge.svg)](https://github.com/jcs-elpa/message-clean-mode/actions/workflows/test.yml)

Simple minor-mode to keep your `*Messages*` buffer clean, without Emacs spamming
a bunch of command messages.

This is only useful for people who constantly check `*Messages*` buffer for debug log.

## 🔨 Usage

First, assign commands you want to keep the `*Messages*` buffer clean.

```el
(setq message-clean-mode-mute-commands '(push-mark ...))
(setq message-clean-mode-echo-commands '(set-mark-command ...))
```

Then call `M-x message-clean-mode`!

```el
(setq message-clean-mode-minor-mode 'echo)  ; or `nil' or `mute'
```

This will allow you to mute message like `xxx-minor-mode is enabled/disabled`!

## Contribute

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Elisp styleguide](https://img.shields.io/badge/elisp-style%20guide-purple)](https://github.com/bbatsov/emacs-lisp-style-guide)
[![Donate on paypal](https://img.shields.io/badge/paypal-donate-1?logo=paypal&color=blue)](https://www.paypal.me/jcs090218)

If you would like to contribute to this project, you may either
clone and make pull requests to this repository. Or you can
clone the project and establish your own branch of this tool.
Any methods are welcome!
