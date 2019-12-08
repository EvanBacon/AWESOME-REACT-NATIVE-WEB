---
description: >-
  React Native for web provides access to browser-only style properties. The following styles apply to any primitive that extends `ViewStylePropTypes` like Text, Image, TextInput, ScrollView, etc...
---

# View Styles

## The API

### [backdropFilter](https://developer.mozilla.org/en-US/docs/Web/CSS/backdrop-filter)

The `backdropFilter` CSS property lets you apply graphical effects such as blurring or color shifting to the area behind an element. Because it applies to everything behind the element, to see the effect you must make the element or its background at least partially transparent.

#### **Type:** `string`

#### Conversion

```
// CSS
background-filter: brightness(60%);

// React Native
backdropFilter: "brightness(60%)",
```

### [backgroundAttachment](https://developer.mozilla.org/en-US/docs/Web/CSS/background-attachment)

The `backgroundAttachment` CSS property sets whether a background image's position is fixed within the viewport, or scrolls with its containing block.

#### **Type:** `string`

#### Conversion

```
// CSS
background-attachment: todo;

// React Native
backgroundAttachment: "todo",
```

### [backgroundBlendMode](https://developer.mozilla.org/en-US/docs/Web/CSS/background-blend-mode)

The `backgroundBlendMode` CSS property sets how an element's background images should blend with each other and with the element's background color.

#### **Type:** `string`

#### Conversion

```
// CSS
background-blend-mode: todo;

// React Native
backgroundBlendMode: "todo",
```

### [backgroundClip](https://developer.mozilla.org/en-US/docs/Web/CSS/background-clip)

The `backgroundClip` CSS property sets whether an element's background extends underneath its border box, padding box, or content box.

#### **Type:** `string`

#### Conversion

```
// CSS
background-clip: todo;

// React Native
backgroundClip: "todo",
```

### [backgroundImage](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image)

The `backgroundImage` CSS property sets one or more background images on an element.

#### **Type:** `string`

#### Conversion

```
// CSS
background-image: todo;

// React Native
backgroundImage: "todo",
```

### [backgroundOrigin](https://developer.mozilla.org/en-US/docs/Web/CSS/background-origin)

The `backgroundOrigin` CSS property sets the background's origin: from the border start, inside the border, or inside the padding.

#### **Type:** `enum('border-box', 'content-box', 'padding-box')`

#### Conversion

```
// CSS
background-origin: todo;

// React Native
backgroundOrigin: "todo",
```

### [backgroundPosition](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)

The `backgroundPosition` CSS property sets the initial position for each background image. The position is relative to the position layer set by `backgroundOrigin`.

#### **Type:** `string`

#### Conversion

```
// CSS
background-position: 50%;

// React Native
backgroundPosition: "50%",
```

### [backgroundRepeat](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat)

The `backgroundRepeat` CSS property sets how background images are repeated. A background image can be repeated along the horizontal and vertical axes, or not repeated at all.

#### **Type:** `string`

#### Conversion

```
// CSS
background-repeat: todo;

// React Native
backgroundRepeat: "todo",
```

### [backgroundSize](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size)

The `backgroundSize` CSS property sets the size of the element's background image. The image can be left to its natural size, stretched, or constrained to fit the available space.

#### **Type:** `string`

#### Conversion

```
// CSS
background-size: todo;

// React Native
backgroundSize: "todo",
```

### [boxShadow](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)

The `boxShadow` CSS property adds shadow effects around an element's frame. You can set multiple effects separated by commas. A box shadow is described by X and Y offsets relative to the element, blur and spread radii, and color.

#### **Type:** `string`

#### Conversion

```
// CSS
box-shadow: todo;

// React Native
boxShadow: "todo",
```

### [clip](https://developer.mozilla.org/en-US/docs/Web/CSS/clip)

The `clip` CSS property defines what portion of an element is visible. The `clip` property applies only to absolutely positioned elements, that is elements with `position: "absolute"` or `position: "fixed"`.

#### **Type:** `string`

#### Conversion

```
// CSS
clip: todo;

// React Native
clip: "todo",
```

### [filter](https://developer.mozilla.org/en-US/docs/Web/CSS/filter)

The `filter` CSS property applies graphical effects like blur or color shift to an element. Filters are commonly used to adjust the rendering of images, backgrounds, and borders.

#### **Type:** `string`

#### Conversion

```
// CSS
fliter: todo;

// React Native
filter: "todo",
```

### [outlineColor](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-color)

An outline is a line that is drawn around elements (outside the borders) to make the element "stand out".

The `outlineColor` property specifies the color of an outline.

> **Note:** Always declare the `outlineStyle` property before the `outlineColor` property. An element must have an outline before you change the color of it.

#### **Type:** `ColorPropType`

#### Conversion

```
// CSS
outline-color: todo;

// React Native
outlineColor: "todo",
```

### [outlineOffset](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-offset)

The `outlineOffset` CSS property sets the amount of space between an outline and the edge or border of an element.

#### **Type:** `enum(string, number)`

#### Conversion

```
// CSS
outline-offset: todo;

// React Native
outlineOffset: "todo",
```

### [outlineStyle](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-style)

An outline is a line that is drawn around elements (outside the borders) to make the element "stand out".

#### **Type:** `string`

#### Conversion

```
// CSS
outline-style: todo;

// React Native
outlineStyle: "todo",
```

### [outlineWidth](https://developer.mozilla.org/en-US/docs/Web/CSS/outline-width)

An outline is a line that is drawn around elements (outside the borders) to make the element "stand out".

> **Note:** Always declare the `outlineStyle` property before the `outlineWidth` property. An element must have an outline before you change the width of it.

#### **Type:** `enum(string, number)`

#### Conversion

```
// CSS
outline-width: todo;

// React Native
outlineWidth: "todo",
```

### [overscrollBehavior](https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior)

The `overscrollBehavior` CSS property sets what a browser does when reaching the boundary of a scrolling area. It's a shorthand for `overscrollBehaviorX` and `overscrollBehaviorY`.

#### **Type:** `enum('auto', 'contain', 'none')`

#### Conversion

```
// CSS
overscroll-behavior: auto;

// React Native
overscrollBehavior: "auto",
```

### [overscrollBehaviorX](https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior-x)

The `overscrollBehaviorX` CSS property sets the browser's behavior when the horizontal boundary of a scrolling area is reached.

#### **Type:** `enum('auto', 'contain', 'none')`

#### Conversion

```
// CSS
overscroll-behavior-x: contain;

// React Native
overscrollBehaviorX: "contain",
```

### [overscrollBehaviorY](https://developer.mozilla.org/en-US/docs/Web/CSS/overscroll-behavior-y)

The `overscrollBehaviorY` CSS property sets the browser's behavior when the vertical boundary of a scrolling area is reached.

#### **Type:** `enum('auto', 'contain', 'none')`

#### Conversion

```
// CSS
overscroll-behavior-y: contain;

// React Native
overscrollBehaviorY: "contain",
```

### [scrollbarWidth](https://developer.mozilla.org/en-US/docs/Web/CSS/scrollbar-width)

The `scrollbarWidth` property allows the author to set the maximum thickness of an element’s scrollbars when they are shown.

#### **Type:** `enum('auto', 'thin', 'none')`

#### Conversion

```
// CSS
scrollbar-width: todo;

// React Native
scrollbarWidth: "todo",
```

### [scrollSnapAlign](https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-snap-align)

The `scrollSnapAlign` property specifies the box’s snap position as an alignment of its snap area (as the alignment subject) within its snap container’s snapport (as the alignment container). The two values specify the snapping alignment in the block axis and inline axis, respectively. If only one value is specified, the second value defaults to the same value.

#### **Type:** `string`

#### Conversion

```
// CSS
scroll-snap-align: todo;

// React Native
scrollSnapAlign: "todo",
```

### [scrollSnapType](https://developer.mozilla.org/en-US/docs/Web/CSS/scroll-snap-type)

The `scrollSnapType` CSS property sets how strictly snap points are enforced on the scroll container in case there is one.

#### **Type:** `string`

#### Conversion

```
// CSS
scroll-snap-type: todo;

// React Native
scrollSnapType: "todo",
```

### [WebkitMaskImage](https://developer.mozilla.org/en-US/docs/Web/CSS/mask-image)

The `maskImage` CSS property sets the image that is used as mask layer for an element.

#### **Type:** `string`

#### Conversion

```
// CSS
text-indent: todo;

// React Native
textIndent: "todo",
```

### [WebkitOverflowScrolling](https://developer.mozilla.org/en-US/docs/Web/CSS/-webkit-overflow-scrolling)

The `WebkitOverflowScrolling` CSS property controls whether or not touch devices use momentum-based scrolling for a given element.

#### **Type:** `enum('auto', 'touch')`

#### Conversion

```
// CSS
text-indent: todo;

// React Native
textIndent: "todo",
```
