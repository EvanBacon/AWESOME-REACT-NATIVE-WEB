---
description: >-
  React Native for web adds the following features to the React Native <TextInput /> element.
---

# TextInput

## Props

### [draggable](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/draggable)

Can the user drag the element around. If this attribute is not set, its default value is auto, which means drag behavior is the default browser behavior: only text selections, images, and links can be dragged.

#### **Type:** `boolean`

#### **Default:** `true`

#### Conversion

```diff
// HTML
- <input draggable="true" />

// React Native
+ <TextInput draggable />
```

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
