### tmux

`C-d` writes an EOF (end of file) to the stdin, which closes the shell
#### Understanding note

When you see `C-*` C = ctrl, * = any key. So the previous example is Control + d.

```text
tmux list-sessions

# If you got excited
tmux kill-server
```

```text
tmux a
tmux attach
```

Prefix Key

- The key combo you press (default `C-b`).

```text
tmux new-session -d
```

#### Navigation tip

I don't use this personal, but this is a thing that is good to know.

- to the next session `<prefix>-(`
- to the prev session `<prefix>-)`

for detach from a session `<prefix>-d`

### Navigation tip

You can see all of the sessions and their windows by pressing `<prefix>-w`

### Creating Windows

```text
tmux
tmux new-window
```

this is equivalent to `<prefix>-c`

#### Navigation tip

- `<prefix>-n` for next window
- `<prefix>-p` for prev window
- `<prefix>-#` for the # window


### Cheat Sheet

Cheat sheet has a lot to offer! Not only just questions about languages but tons of examples around core utils, language specifics, and a TL/DR on learning languages.

```text
curl cht.sh/find~exec
```

```text
curl cht.sh/javascript/splice+array
```

```text
curl cht.sh/typescript/enum
```

```text
curl cht.sh/typescript/enum+string
```

COPY PASTE
#### Usability Tip

`<prefix>-[` goes into vi mode

this for the copy/paste in tmuxrc

```text
set-window-option -g mode-keys vi
bind -T copy-mode-vi v send-keys -X begin-selection
bind -T copy-mode-vi y send-keys -X copy-pipe-and-cancel 'xclip -in -selection clipboard'
```