# Where's DigitalCrafts?

This program displays the states which have cities named "Atlanta", "Houston", "Tampa".

# Bugs to fix

- [x] After lots of debugging, code stopped running. `node index.js` does nothing
- [x] Started crashing after adding "tampa" search
- [x] Prints "Atlanta" locations twice (instead of Houston)

For each bug you fix, add documentation to this README about how you fixed it (include before/after code samples).

# For the more curious:

`db.js` includes more functions that you can try out. In `index.js`, try to `console.log()` the results of the following function calls:

- `getByAbbreviation('ak')`
- `searchByName('dakota')`
- Why does this only return results for North Dakota (and not South Dakota)?

# Documentation one how I fixed the bugs

- When I ran `index.js` using `node` nothing happened, I saw that the function `main()` was commented out and it could have ment that it wasn't running that function hence not running the programming , I uncomment the code, and the program ran causing the second bug to happen.

- When I saw the error `ReferenceError: statesWithCity is not defined` I knew that something wasn't right and read more on the error and it said ` const statesWithATampa = statesWithCity("tampa");` and I saw that the `db.` wasn't in front of the callback.

- The reason that the Houston loop was printing the Atlanta was because it was calling the `statesWithAnAtlanta` instead of
