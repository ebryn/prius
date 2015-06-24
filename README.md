
# Prius

Prius enables you to write next generation CSS in your apps today. It operates via a hybrid runtime and preprocessor. 
Prius is currently intended for usage inside Ember CLI applications, however it was built to be used with any JS framework.

## Demo

<img src="http://g.recordit.co/5TGVaKLbLv.gif">

## Installation

`ember install prius`

Add `{{prius-meta}}` to the `<head>` of your [`app/index.html`](https://github.com/ebryn/prius/blob/master/tests/dummy/app/index.html#L15) & [`tests/index.html`](https://github.com/ebryn/prius/blob/master/tests/index.html#L17)

TODO: instructions for general usage.

## Features

### CSS custom properties and `var`

#### Example usage

```
.button {
  font-size: var(--fontSize, 1em);
}

.button-large {
  --fontSize: 2em;
}
```

## Planned features

### Mixins

#### Example usage

```
:root {
  --myMixin: {
    padding: 0.5em;
  }
}

.button {
  @apply(--myMixin)
}
```
