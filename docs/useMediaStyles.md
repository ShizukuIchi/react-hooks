# `useMediaStyles`

React hook returns a style object from specified media queries and styles.

Style changes due to viewport size.

## Usage

```jsx
import { useState } from 'react';
import useMediaStyles from 'src/useMediaStyles';

const Demo = () => {
  const style = useMediaStyles({
    '(max-width: 600px)': {
      background: 'red',
    },
    '(min-width: 601px)': {
      background: 'blue',
    },
  });
  return <div style={style} />;
};
```

## Reference

```jsx
useMediaStyles(mediaQueryOptions);
```

- `mediaQueryOptions`
  - `mediaQuery` &mdash; a media query string
    - `style` &mdash; a style object
