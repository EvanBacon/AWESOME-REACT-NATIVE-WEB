---
description: null
---

# Aspect Ratio

Because the `aspectRatio` style prop isn't available in `react-native-web`'s StyleSheet API, we need to improvise a bit.

### [Snack](https://snack.expo.io/@bacon/aspectratio)

```jsx
import * as React from 'react';
import { Text, View, StyleSheet } from 'react-native';

function AspectView(props) {
  const [layout, setLayout] = React.useState(null);

  const { aspectRatio = 1, ...inputStyle } =
    StyleSheet.flatten(props.style) || {};
  const style = [inputStyle, { aspectRatio }];

  if (layout) {
    const { width = 0, height = 0 } = layout;
    if (width === 0) {
      style.push({ width: height * aspectRatio, height });
    } else {
      style.push({ width, height: width * aspectRatio });
    }
  }

  return (
    <View
      {...props}
      style={style}
      onLayout={({ nativeEvent: { layout } }) => setLayout(layout)}>
      {layout ? props.children : null}
    </View>
  );
}

// ...

return <AspectView style={{ width: 48, aspectRatio: 0.75 }} />;
```

<div data-snack-id="@bacon/aspectratio" data-snack-platform="web" data-snack-preview="true" data-snack-theme="light" style="overflow:hidden;background:#fafafa;border:1px solid rgba(0,0,0,.08);border-radius:4px;height:505px;width:100%"></div>
<script async src="https://snack.expo.io/embed.js"></script>
