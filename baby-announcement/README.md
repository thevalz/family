# Baby announcement — interaction study

A single, self-contained animated web page exploring how our baby-name
announcement could feel to play with. This is a **design study**, not the
finished page: it presents five interactive concepts side by side so we can
react to them and pick a direction to iterate on.

Open `index.html` in any browser — no build step, no dependencies (the display
font is inlined as a data URI, so it works offline and anywhere).

## The five ideas

| # | Concept | Interaction |
|---|---------|-------------|
| 01 | **Lantern Field** | Balloons lean away from the cursor and part like a curtain, with parallax depth. |
| 02 | **Petal Trail** | The cursor leaves a wake of warm petals that rise and fade. |
| 03 | **The Name Plays** | The name's letters lean toward the cursor, warm and glow, then spring back. |
| 04 | **Golden Spotlight** | A warm light travels with the cursor, revealing a hidden message. |
| 05 | **Pop to Reveal** | Hover or tap each balloon to pop it and uncover a letter of the name. |

## Look & feel

"Golden-hour dusk" — earthy balloons (terracotta, ochre, sage, clay, dusty
rose, plum) glowing like paper lanterns against a warm ground. Works in both
light and dark themes; there's a toggle in the top-right corner.

## Swapping in the real name

Everything configurable lives in one object at the top of the `<script>` in
`index.html`:

```js
const BABY = {
  name: "Baby Valz",                  // <- the real name
  popLetters: ["V","A","L","Z"],      // letters for the "Pop to Reveal" idea
  spotMessage: "we already can't wait to meet you",
};
```

The name is currently a clearly-marked placeholder.
