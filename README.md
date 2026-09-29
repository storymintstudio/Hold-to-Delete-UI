# Hold to Delete

A press-and-hold delete confirmation for file/list UIs — no popup, no accidental clicks. Hold the button, watch the fill and shake build, and the item shatters away when the hold completes.

![type](https://img.shields.io/badge/type-UI%20component-c8ff00?style=flat-square)
![stack](https://img.shields.io/badge/stack-HTML%2FCSS%2FJS-111?style=flat-square)

## Demo

Open `index.html` in any browser, or drop it into a Live Server.

## Features

- Press-and-hold confirm pattern — replaces `confirm()` / `alert()` dialogs
- Radial fill + label progress (`0% → 100%`) while holding
- Row shake feedback during the hold
- Particle "shatter" burst + collapse animation on delete
- Full keyboard support (`Space` / `Enter` to hold, release to cancel)
- Respects `prefers-reduced-motion`
- Empty-state message once all items are cleared, with a restore button for re-testing
- Zero dependencies — vanilla HTML/CSS/JS, single file

## Usage

Just open `index.html`. To use it in your own project, copy the `.row` / `.del` markup pattern and the `wire()` function, and swap `FILES` for your own data source.

```js
const FILES = [["filename.ext", "size"], ...];
```

Each row wires up its own hold state via Pointer Events, so it works the same on touch and mouse.

## Customize

- `HOLD` (ms) in the script — how long the press must be held
- `--danger`, `--card`, `--line`, `--ring` CSS variables — color theme
- Background image/gradient — set in the `body` rule

## Credits

First draft generated with AI, customized and crafted by Storymint Studio.

---

Built by [@storymint.studio](https://instagram.com/storymint.studio) — new UI drop every week.
