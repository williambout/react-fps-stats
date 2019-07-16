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

const Application = () => {
  return (
    <div>
      <FPSStats />
    </div>
  );
};

render(<Application />, document.body);
```

### Optional Props

By default, the meter is fixed positioned in the top left of the screen. You can pass the optional props `top`, `right`, `bottom` & `left` to overrride that positioning. Each prop maps to the css values and can use either string or number format. `top` and `left` have values by default, so pass `'auto'` as their values if you want to use `bottom` or `right` values.

## Alternatives

If you are only using this for development purpose and your users don't need to see it, you can consider using the [Chrome Devtools FPS Meter](https://developer.chrome.com/devtools/docs/rendering-settings#show-fps%20meter).
