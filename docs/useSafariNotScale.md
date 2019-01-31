# `useSafariNotScale`

React hook prevents webpage scaling in safari.

iOS 10, 11, 12 safari DO NOT respect the `user-scalable=no` meta tag. User can still zoom the webpage by pinching or double tapping.

## Usage

```jsx
import useSafariNotScale from 'src/useSafariNotScale';

const Demo = () => {
  useSafariNotScale();
  return 'Scaling Disabled';
};
```
