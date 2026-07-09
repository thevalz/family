# Baby announcement

A single, self-contained animated web page announcing our baby's name — a room
full of balloons that float up from the floor, collect at the ceiling, bump
into each other, and scatter when you move your cursor through them.

Open `index.html` in any browser — no build step, no dependencies (the display
font is inlined as a data URI, so it works offline and anywhere).

## The scene

- On load, the balloons start at the **bottom** of the screen.
- Helium **buoyancy** carries them up; they collect along the top like a garland.
- A lightweight **physics** loop keeps them from overlapping — balloons separate
  and bounce off each other and the walls.
- Your **cursor** pushes nearby balloons around; released, they drift back up.

Balloons are rendered as realistic glossy latex (in the spirit of the Cotton
launch campaign) — volumetric shading, a hot-spot highlight, a knot and a
dangling string.

## Two palettes

Use the switch in the top-right corner to compare:

- **Bright Sky** (default) — candy-colored balloons on a sunny sky.
- **Golden Dusk** — earthy balloons against a warm, moody ground.

The choice persists across reloads.

## Swapping in the real name

Everything configurable is one line at the top of the `<script>` in
`index.html`:

```js
const BABY = { name: "Baby Valz" };   // <- the real name
```

The name is currently a clearly-marked placeholder.
