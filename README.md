# zathurarc

Dark blue theme for [zathura](https://pwmt.org/projects/zathura/). Deep navy canvas, soft blue accent, light grey text.

## Palette

| Role               | Color     |
|--------------------|-----------|
| Canvas background  | `#121923` |
| Foreground         | `#e9eaed` |
| Bars / index bg    | `#121519` |
| Input bar / group  | `#181c22` |
| Completion bg      | `#1c2027` |
| Notification bg    | `#1f252d` |
| Accent             | `#a0bbe3` |
| Accent text (on accent) | `#0c1f3b` |
| Error bg / fg      | `#8c1d18` / `#f9dedc` |
| Warning fg         | `#e8c26a` |

## What it styles

- Reading canvas and recolor (dark mode for PDFs)
- Status bar and input bar
- Completion menu
- Notifications (info, warning, error)
- Index / table of contents
- Search highlights (accent at 15% / 30% alpha)
- Loading state

It also sets `selection-clipboard clipboard` so selections go to the system clipboard.

## Install

```sh
mkdir -p ~/.config/zathura
cp zathurarc ~/.config/zathura/zathurarc
```

Or symlink:

```sh
ln -sf "$PWD/zathurarc" ~/.config/zathura/zathurarc
```

Restart zathura.

## Notes

- `recolor` is on by default. Toggle in zathura with `Ctrl+r` for original PDF colors.
- Colors use `rgba(r,g,b,a)` syntax, with hex noted in comments. Edit the accent in one place per role to retheme.
