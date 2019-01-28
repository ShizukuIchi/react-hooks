# `useMediaStyles`

React hook generates a resettable setTimeout and only reset when reset is invoked.

## Usage

```jsx
import { useState } from 'react';
import useResettableTimeout from 'src/useResettableTimeout';

const Demo = () => {
  const [ready, setReady] = useState(true);
  const reset = useResettableTimeout(1000, setReady, false);
  return <div onClick={reset}>Are you ready? {ready ? 'Yes' : 'No'}</div>;
};
```

## Reference

```jsx
useResettableTimeout(ms, callback, args);
```

- `ms` &mdash; time in milliseconds to invoke callback, default to `0`.
- `callback` &mdash; function to invoke after timeout.
- `args` &mdash; arguments for the callback, default to `[]`.
