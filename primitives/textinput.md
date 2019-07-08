---
description: >-
  React Native for web adds the following features to the React Native
  <TextInput /> element.
---

# TextInput

## Props

### [caretColor](https://developer.mozilla.org/en-US/docs/Web/CSS/caret-color)

Sets the color of the insertion caret, the visible marker where the next character typed will be inserted. The caret is typically a thin vertical line that flashes to help make it more noticeable.

#### **Type:** `ColorPropType`

#### Conversion

```diff
// HTML & CSS
- <input style="caret-color: red;" />

// React Native
+ <TextInput caretColor="red" />
```

### [resize](https://developer.mozilla.org/en-US/docs/Web/CSS/resize)

Whether an element is resizable, and if so, in which directions.

#### **Type:** `'none' | 'vertical' | 'horizontal' | 'both'`

#### **Default:** `'none'`

#### Conversion

```diff
// HTML & CSS
- <textarea style="resize: both;" />

// React Native
+ <TextInput resize="both" />
```

