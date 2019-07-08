---
description: >-
  React Native for web provides access to browser-only style properties. The
  following styles apply to any primitive that extends `TextViewStylePropTypes`
  like `<TextInput />`.
---

# Text

## The API

### [textIndent](https://developer.mozilla.org/en-US/docs/Web/CSS/text-indent)

Sets the length of empty space \(indentation\) that is put before lines of text in a block.

#### **Type:** `number | string`

#### Conversion

```diff
// CSS
- text-indent: 30px;

// React Native
+ textIndent: 30,
```

### [textOverflow](https://developer.mozilla.org/en-US/docs/Web/CSS/text-overflow)

Sets how hidden overflow content is signaled to users. It can be clipped, display an ellipsis \('`…`'\), or display a custom string.

#### **Type:** `string | 'each-line' | 'hanging' | Array<T>`

#### Conversion

```diff
// CSS
- text-overflow: 5px hanging each-line;

// React Native
+ textOverflow: [5, "hanging", "each-line"],
```

### [textRendering](https://developer.mozilla.org/en-US/docs/Web/CSS/text-rendering)

Provides information to the rendering engine about what to optimize for when rendering text. The browser makes trade-offs among speed, legibility, and geometric precision.

#### **Type:** `'auto' | 'geometricPrecision' | 'optimizeLegibility' | 'optimizeSpeed'`

#### Conversion

```diff
// CSS
- text-rendering: optimizeLegibility;

// React Native
+ textRendering: "optimizeLegibility",
```

### [unicodeBidi](https://developer.mozilla.org/en-US/docs/Web/CSS/unicode-bidi)

The **`unicodeBidi`** property, together with the `direction` property, determines how bidirectional text in a document is handled. For example, if a block of content contains both left-to-right and right-to-left text, the user-agent uses a complex Unicode algorithm to decide how to display the text. The `unicodeBidi` property overrides this algorithm and allows the developer to control the text embedding.

#### **Type:** `'normal','bidi-override','embed','isolate','isolate-override','plaintext'`

#### Conversion

```diff
// CSS
- unicode-bidi: embed;

// React Native
+ unicodeBidi: "embed",
```

### [whiteSpace](https://developer.mozilla.org/en-US/docs/Web/CSS/white-space)

Sets how [white space](https://developer.mozilla.org/en-US/docs/Glossary/whitespace) inside an element is handled. **Note:** To make words break _within themselves_, use [`overflow-wrap`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow-wrap), [`word-break`](https://developer.mozilla.org/en-US/docs/Web/CSS/word-break), or [`hyphens`](https://developer.mozilla.org/en-US/docs/Web/CSS/hyphens) instead.

#### **Type:** `string`

#### Conversion

```diff
// CSS
- white-space: word-break;

// React Native
+ whiteSpace: "word-break",
```

### [wordBreak](https://developer.mozilla.org/en-US/docs/Web/CSS/word-break)

Sets whether line breaks appear wherever the text would otherwise overflow its content box.

#### **Type:** `'normal', 'break-all', 'break-word', 'keep-all'`

#### Conversion

```diff
// CSS
- word-break: break-all;

// React Native
+ wordBreak: "break-all",
```

### [wordWrap](https://developer.mozilla.org/en-US/docs/Web/CSS/word-wrap)

Applies to inline elements, setting whether the browser should insert line breaks within an otherwise unbreakable string to prevent text from overflowing its line box.

> In CSS `word-wrap` is also known as `overflow-wrap`

#### **Type:** `'normal' | 'anywhere' | 'break-word'`

#### Conversion

```diff
// CSS
- word-wrap: anywhere;

// React Native
+ wordWrap: "anywhere",
```

### [WebkitFontSmoothing](https://developer.mozilla.org/en-US/docs/Web/CSS/font-smooth)

### [MozOsxFontSmoothing](https://developer.mozilla.org/en-US/docs/Web/CSS/font-smooth)

Controls the application of anti-aliasing when fonts are rendered.

#### **Type:** `string`

#### Conversion

```diff
// CSS
- font-smooth: always;

// React Native
+ WebkitFontSmoothing: "always",
+ MozOsxFontSmoothing: "always",
```

