[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![JCS-ELPA](https://raw.githubusercontent.com/jcs-emacs/badges/master/elpa/v/message-clean-mode.svg)](https://jcs-emacs.github.io/jcs-elpa/#/message-clean-mode)

# message-clean-mode
> Keep messages buffer clean

[![CI](https://github.com/jcs-elpa/message-clean-mode/actions/workflows/test.yml/badge.svg)](https://github.com/jcs-elpa/message-clean-mode/actions/workflows/test.yml)

Simple minor-mode to keep your `*Messages*` buffer clean, without Emacs spamming
a bunch of command messages.

*P.S. This is only useful for people who constantly check `*Messages*` buffer
for debug log.*

## 💾 Quickstart

```el
(leaf message-clean-mode
  :hook (after-init-hook . message-clean-mode)
  :init
  (setq message-clean-mode-mute-commands '(push-mark set-mark-command)
        message-clean-mode-echo-commands '(mwheel-scroll
                                           previous-line next-line
                                           mark-whole-buffer
                                           indent-region
                                           isearch-done
                                           undefined
                                           toggle-truncate-lines)
        message-clean-mode-minor-mode 'echo))  ; echo minor mode only
```

## Contribute

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Elisp styleguide](https://img.shields.io/badge/elisp-style%20guide-purple)](https://github.com/bbatsov/emacs-lisp-style-guide)
[![Donate on paypal](https://img.shields.io/badge/paypal-donate-1?logo=paypal&color=blue)](https://www.paypal.me/jcs090218)

If you would like to contribute to this project, you may either
clone and make pull requests to this repository. Or you can
clone the project and establish your own branch of this tool.
Any methods are welcome!
