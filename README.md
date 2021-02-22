# var-board

var-board is a JavaScript chessboard component that allows boards of variable dimensions. 
It is based on chessboard.js and depends on [jQuery] v3.4.1 (or higher).

Please see [chessboardjs.com] for documentation and examples.

## What is var-board?

var-board is a standalone JavaScript Chess Board. It is designed to be "just
a board" and expose a powerful API so that it can be used in different ways.
Here's a non-exhaustive list of things you can do with var-board:

- Use var-board to show game positions alongside your expert commentary.
- Use var-board to have a tactics website where users have to guess the best
  move.
- Integrate var-board and [chess.js] with a PGN database and allow people to
  search and playback games (see [Example 5000])
- Build a chess server and have users play their games out using the
  var-board board.

var-board is flexible enough to handle any of these situations with relative
ease.

## What can var-board **not** do?

The scope of var-board is limited to "just a board." This is intentional and
makes var-board flexible for building a variety of chess-related
applications.

To be specific, var-board does not understand anything about how the game of
chess is played: how a knight moves, whose turn is it, is White in check?, etc.

Fortunately, the [chess.js] library deals with exactly this sort of problem and
plays nicely with var-board's flexible API. Some examples of var-board
combined with chess.js: [Example 5000], [Example 5001], [Example 5002]

## Docs and Examples

- Docs - <https://chessboardjs.com/docs>
- Examples - <https://chessboardjs.com/examples>

- Custom dimensions example: 
```
var config = {
  rows: '6',
  columns: '16'
}
var board = Chessboard('myBoard', config)
```
## Developer Tools

```sh
# create a build in the build/ directory
npm run build

# re-build the website
npm run website
```

## License

[MIT License](LICENSE.md)

[jQuery]:https://jquery.com/
[chessboardjs.com]:https://chessboardjs.com
[chess.js]:https://github.com/jhlywa/chess.js
[Example 5000]:https://chessboardjs.com/examples#5000
[Example 5001]:https://chessboardjs.com/examples#5001
[Example 5002]:https://chessboardjs.com/examples#5002
