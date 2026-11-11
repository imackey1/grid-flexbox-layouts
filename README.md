# In-Class 04: Grid and Flexbox

Two layout exercises: a recipe page built with Flexbox and a Tic-Tac-Toe board built with CSS Grid.

**Author:** Ibrahim Mackey
**Live pages (CODD):**
- Recipe: https://codd.cs.gsu.edu/~imackey1/web/INC/INC4/recipe.html
- Tic-Tac-Toe: https://codd.cs.gsu.edu/~imackey1/web/INC/INC4/tictactoe.html

## Part 1: Recipe with Flexbox
- `header`: `display: flex; justify-content: space-between` (logo and title on opposite sides)
- `.content` and `.main-content`: flex containers with `flex-wrap: wrap`; `.main-content` grows with `flex-basis: 70%`
- `.title`: `align-items: baseline` so mixed font sizes share a baseline
- `.summary`: `justify-content: space-evenly`, `flex-grow: 1`, `flex-basis: 100%`; its inner `div > div` uses `space-between`
- `.ingredients` and `.directions`: `flex-grow: 1; flex-basis: 45%`; `.related-content`: `flex-basis: 20%`
- Cookie image has `box-shadow` and `border-radius`

## Part 2: Tic-Tac-Toe with Grid
- `#board`: `display: grid`, three 100px columns and rows (`repeat(3, 100px)`), `gap: 10px`, `justify-content: center`
- Squares use `display: flex` to center the X or O, plus a background, border and hover effect

## Files
| File | Purpose |
|------|---------|
| `recipe.html`, `recipe.css` | Flexbox recipe page |
| `cookie.svg` | Cookie image used in the sidebar |
| `tictactoe.html`, `tictactoe.css` | Grid board |
