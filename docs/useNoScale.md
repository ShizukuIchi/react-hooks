# `useNoScale`

React hook prevents webpage scaling by gestures in mobile devices.

iOS 10, 11, 12 safari DO NOT respect the `user-scalable=no` meta tag. User can still zoom the webpage by pinching or double tapping.

## Usage

```jsx
import useNoScale from 'src/useNoScale';

const Demo = () => {
  useNoScale();
  return 'Scaling Disabled';
};
```
