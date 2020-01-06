---
description: Universal solution to the missing aspect ratio prop
---

# Aspect Ratio

Because the `aspectRatio` style prop isn't available in `react-native-web`'s StyleSheet API, we need to improvise a bit. Here is a `View` which accepts an `aspectRatio` style prop and calculates the ratio for you!

## Example [Snack](https://snack.expo.io/@bacon/aspectratio)

{% embed url="https://snack.expo.io/@bacon/aspectratio" %}

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

