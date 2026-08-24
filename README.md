# tmux-config

My minimal tmux configuration for keyboard-driven terminal work across Linux hosts and mobile/remote sessions.

## Features

* Vim-style copy mode
* `v` to begin selection
* `y` to copy using tmux/OSC 52
* `Y` to copy directly to an X11 clipboard using `xclip`
* OSC 52 support works well with compatible terminals such as Blink Shell on iOS

## Install

```bash
wget -qO ~/.tmux.conf \
  https://raw.githubusercontent.com/wz3rd/tmux-config/main/.tmux.conf
```

Reload an existing tmux session with:

```bash
tmux source-file ~/.tmux.conf
```

`xclip` is only required for the optional `Y` X11 clipboard binding.

## License

Released under The Unlicense. Use it however you want.
