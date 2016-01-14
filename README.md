# palette

Color palette variables
  
## Usage

```stylus

// a bright blue button
.button-blue
  %concerted/palette/index.ess

   // we can change the hue, saturation, or lightness
  --palette-1-h 200
  --palette-1-l 75%
  background-color var(--palette-1)

  &:hover
    background-color var(--palette-1-light)

// best of all, the properties cascade.
// this inner icon has the same access to its
// parent variables
.button-blue-icon
  border 0 1px var(--palette-1-dark)

// a dark red button using red variable
.button-red
  %concerted/palette/index.ess

  --palette-1 var(--palette-red-dark)
  background-color var(--palette-1)

// or, to set the variables globally
:root
  %concerted/palette/index.ess
```

## License

MIT
