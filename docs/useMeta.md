# `useMeta`

React hook sets meta tag of the page.

Meta tag will be restore after unmounted.

## Usage

```jsx
import useMeta from 'src/useMeta';

const Demo = () => {
  useMeta('viewport', {
    content: '',
  });
  return <div>viewport changed</div>;
  // <meta name="viewport" content="" />
};
```

## Reference

```jsx
useMeta(name, options);
```

- `name` &mdash; the meta tag name to set
- `options`
  - `attribute` &mdash; the attribute to set
  - `value` &mdash; the value of the attribute
