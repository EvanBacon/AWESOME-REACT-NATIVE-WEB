---
description: null
---

# Interactions

## Props

### [cursor](https://developer.mozilla.org/en-US/docs/Web/CSS/cursor)

Sets the type of cursor, if any, to show when the mouse pointer is over an element.

#### **Type:** `string`

#### Conversion

```diff
// CSS
- cursor: help;

// React Native
+ cursor: "help",
```

### [userSelect](https://developer.mozilla.org/en-US/docs/Web/CSS/user-select)

Controls whether the user can select text. This doesn't have any effect on content loaded as [chrome](https://developer.mozilla.org/en-US/docs/Glossary/Chrome), except in textboxes.

#### **Type:** `string`

#### Conversion

```diff
// CSS
- user-select: text;

// React Native
+ userSelect: "text",
```

### [willChange](https://developer.mozilla.org/en-US/docs/Web/CSS/will-change)

Hints to browsers how an element is expected to change. Browsers may set up optimizations before an element is actually changed. These kinds of optimizations can increase the responsiveness of a page by doing potentially expensive work before they are actually required.

#### **Type:** `string`

#### Conversion

```diff
// CSS
- will-change: transform;

// React Native
+ willChange: "transform",
```

### [touchAction](https://developer.mozilla.org/en-US/docs/Web/CSS/touch-action)

Sets how an element's region can be manipulated by a touchscreen user \(for example, by zooming features built into the browser\).

#### **Type:** `'auto' | 'inherit' | 'manipulation' | 'none' | 'pan-down' | 'pan-left' | 'pan-right' | 'pan-up' | 'pan-x' | 'pan-y' | 'pinch-zoom'`

#### Conversion

```diff
// CSS
- touch-action: pan-down;

// React Native
+ touchAction: "pan-down",
```

