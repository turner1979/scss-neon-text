# SCSS Neon Text

See demo of effect on [Codepen](https://codepen.io/sturner/pen/LYyGpJw)

## Installation

To install do the following:
```
npm i scss-neon-text
```

Next import the ***neon-text.scss*** file where needed e.g:

```
@import '~scss-neon-text/neon-text.scss';
@include neonInit();
```

This will setup the keyframes css needed for the neon effect.

Finally include the neonText mixin where needed in your styles, e.g:

```
h1 {
  @incude neonText();
}
```

## Config

```
$defaultConfig: (
  baseColour: '#fff',
  glowColour: '#f09'
);
```

By default the neon effect is pink, this can be overridden by setting a different glowColour property in the config object, like so:

```
$config: (
  glowColour: '#66ff00'
);

@include neonMixin($config);
```
