# React FPS Stats

## Graphics Performance Monitor for React

Forked from https://github.com/sebslomski/react-stats, inspired by https://github.com/mrdoob/stats.js.

### Screenshots

![FPS](http://i.imgur.com/nqcXluS.png)

### Usage

```javascript
import React, { Component } from "react";
import { render } from "react-dom";
import FPSStats from "react-fps-stats";

const __DEV__ = true;

const Application = () => {
  return (
    <div>
      <FPSStats isActive={__DEV__} />
    </div>
  );
};

render(<Application />, document.body);
```

### Optional Props

By default, the meter is fixed positioned in the bottom right. You can pass the
optional props `top`, `right`, `bottom` & `left` to overrride that positioning.
`bottom` & `right` have values by default, so pass `'auto'` as their values if
you want to use `left` or `top` values.
