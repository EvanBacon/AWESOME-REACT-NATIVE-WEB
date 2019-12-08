---
description: >-
  React Native for web provides access to browser-only style properties. The following styles apply to any primitive that extends `ViewStylePropTypes` like Text, Image, TextInput, ScrollView, etc...
---

# View Styles

## The API

### [backdropFilter](https://developer.mozilla.org/en-US/docs/Web/CSS/background-filter)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-filter: todo;

// React Native
+ backdropFilter: "todo",
```

### [backgroundAttachment](https://developer.mozilla.org/en-US/docs/Web/CSS/background-attachment)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-attachment: todo;

// React Native
+ backgroundAttachment: "todo",
```

### [backgroundBlendMode](https://developer.mozilla.org/en-US/docs/Web/CSS/background-blend-mode)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-blend-mode: todo;

// React Native
+ backgroundBlendMode: "todo",
```

### [backgroundClip](https://developer.mozilla.org/en-US/docs/Web/CSS/background-clip)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-clip: todo;

// React Native
+ backgroundClip: "todo",
```

### [backgroundImage](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-image: todo;

// React Native
+ backgroundImage: "todo",
```

### [backgroundOrigin](https://developer.mozilla.org/en-US/docs/Web/CSS/background-origin)

desccc

#### **Type:** `enum('border-box', 'content-box', 'padding-box')`

#### Conversion

```diff
// CSS
- background-origin: todo;

// React Native
+ backgroundOrigin: "todo",
```

### [backgroundPosition](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-position: todo;

// React Native
+ backgroundPosition: "todo",
```

### [backgroundRepeat](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-repeat: todo;

// React Native
+ backgroundRepeat: "todo",
```

### [backgroundSize](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- background-size: todo;

// React Native
+ backgroundSize: "todo",
```

### [boxShadow](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- box-shadow: todo;

// React Native
+ boxShadow: "todo",
```

### [clip](https://developer.mozilla.org/en-US/docs/Web/CSS/clip)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- clip: todo;

// React Native
+ clip: "todo",
```

### [filter](https://developer.mozilla.org/en-US/docs/Web/CSS/fliter)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- fliter: todo;

// React Native
+ filter: "todo",
```

### [outlineColor](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-color)

An outline is a line that is drawn around elements (outside the borders) to make the element "stand out".

The `outlineColor` property specifies the color of an outline.

> **Note:** Always declare the `outlineStyle` property before the `outlineColor` property. An element must have an outline before you change the color of it.

#### **Type:** `ColorPropType`

#### Conversion

```diff
// CSS
- outline-color: todo;

// React Native
+ outlineColor: "todo",
```

### [outlineOffset](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-offset)

desccc

#### **Type:** `enum(string, number)`

#### Conversion

```diff
// CSS
- outline-offset: todo;

// React Native
+ outlineOffset: "todo",
```

### [outlineStyle](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-style)

An outline is a line that is drawn around elements (outside the borders) to make the element "stand out".

#### **Type:** `string`

#### Conversion

```diff
// CSS
- outline-style: todo;

// React Native
+ outlineStyle: "todo",
```

### [outlineWidth](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-width)

An outline is a line that is drawn around elements (outside the borders) to make the element "stand out".

> **Note:** Always declare the `outlineStyle` property before the `outlineWidth` property. An element must have an outline before you change the width of it.

#### **Type:** `enum(string, number)`

#### Conversion

```diff
// CSS
- outline-width: todo;

// React Native
+ outlineWidth: "todo",
```

### [overscrollBehavior](https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior)

The `overscrollBehavior` CSS property sets what a browser does when reaching the boundary of a scrolling area. It's a shorthand for `overscrollBehaviorX` and `overscrollBehaviorY`.

#### **Type:** `enum('auto', 'contain', 'none')`

#### Conversion

```diff
// CSS
- overscroll-behavior: auto;

// React Native
+ overscrollBehavior: "auto",
```

### [overscrollBehaviorX](https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior-x)

The `overscrollBehaviorX` CSS property sets the browser's behavior when the horizontal boundary of a scrolling area is reached.

#### **Type:** `enum('auto', 'contain', 'none')`

#### Conversion

```diff
// CSS
- overscroll-behavior-x: contain;

// React Native
+ overscrollBehaviorX: "contain",
```

### [overscrollBehaviorY](https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior-y)

The `overscrollBehaviorY` CSS property sets the browser's behavior when the vertical boundary of a scrolling area is reached.

#### **Type:** `enum('auto', 'contain', 'none')`

#### Conversion

```diff
// CSS
- overscroll-behavior-y: contain;

// React Native
+ overscrollBehaviorY: "contain",
```

### [scrollbarWidth](https://developer.mozilla.org/en-US/docs/Web/CSS/scrollbar-width)

The scrollbar-width property allows the author to set the maximum thickness of an element’s scrollbars when they are shown.

#### **Type:** `enum('auto', 'thin', 'none')`

#### Conversion

```diff
// CSS
- scrollbar-width: todo;

// React Native
+ scrollbarWidth: "todo",
```

### [scrollSnapAlign](https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-snap-align)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- scroll-snap-align: todo;

// React Native
+ scrollSnapAlign: "todo",
```

### [scrollSnapType](https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-snap-type)

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- scroll-snap-type: todo;

// React Native
+ scrollSnapType: "todo",
```

### WebkitMaskImage

desccc

#### **Type:** `string`

#### Conversion

```diff
// CSS
- text-indent: todo;

// React Native
+ textIndent: "todo",
```

### WebkitOverflowScrolling

desccc

#### **Type:** `enum('auto', 'touch')`

#### Conversion

```diff
// CSS
- text-indent: todo;

// React Native
+ textIndent: "todo",
```
