# KJS BrainFuck Interpreter

[![kjspkg-available](https://github-production-user-asset-6210df.s3.amazonaws.com/79367505/250114674-fb848719-d52e-471b-a6cf-2c0ea6729f1c.svg)](https://kjspkglookup.modernmodpacks.site/#brainfuck-interpreter)

## Docs

Execute bf code:

```js
global.brainfuck("<code here>")
```

Get output:

```js
let bf = global.brainfuck("+[.+]")
console.log(bf.output) // All ascii characters
```

Get other stuff:

```js
let bf = global.brainfuck("+[.+]>++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++.")
console.log(bf.input) // Input code ("+[.+]>++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++.")
console.log(bf.lastCell) // The index of the last cell selected (1)
console.log(bf.cellArray) // The final array of cells ([0, 72, 0, 0, 0...])
```

## Limitations

The `,` character is not supported.
