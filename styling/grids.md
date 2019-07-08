---
description: null
---

# Grids

## The API

## [gridAutoColumns](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-columns)

Specifies the size of an implicitly-created grid column [track](https://developer.mozilla.org/en-US/docs/Glossary/grid_tracks).

### **Type:** `string | number`

### Conversion

```diff
// CSS
- grid-auto-columns: 100px;

// React Native
+ gridAutoColumns: 100,
```

## [gridAutoFlow](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-flow)

Controls how the auto-placement algorithm works, specifying exactly how auto-placed items get flowed into the grid.

### **Type:** `string`

### Conversion

```diff
// CSS
- grid-auto-flow: auto;

// React Native
+ gridAutoFlow: "auto",
```

## [gridAutoRows](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-auto-rows)

Specifies the size of an implicitly-created grid row track.

### **Type:** `string`

### Conversion

```diff
// CSS
- grid-auto-rows: auto;

// React Native
+ gridAutoRows: "auto",
```

## [gridColumnEnd](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-end)

Specifies a grid item’s end position within the grid column by contributing a line, a span, or nothing \(automatic\) to its grid placement, thereby specifying the block-end edge of its [grid area](https://developer.mozilla.org/en-US/docs/Glossary/grid_areas).

### **Type:** `string | number`

### Conversion

```diff
// CSS
- grid-column-end: 2;

// React Native
+ gridColumnEnd: 2,
```

## [gridColumnGap](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-gap)

Sets the size of the gap \([gutter](https://developer.mozilla.org/en-US/docs/Glossary/Gutters)\) between an element's columns.

### **Type:** `string | number`

### Conversion

```diff
// CSS
- grid-column-gap: 8;

// React Native
+ gridColumnGap: 8,
```

## [gridColumnStart](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-column-start)

Specifies a grid item’s start position within the grid column by contributing a line, a span, or nothing \(automatic\) to its grid placement. This start position defines the block-start edge of the [grid area](https://developer.mozilla.org/en-US/docs/Glossary/grid_areas).

### **Type:** `'row' | 'column' | 'dense'`

### Conversion

```diff
// CSS
- grid-column-start: column;

// React Native
+ gridColumnStart: "column",
```

## [gridRowEnd](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-Row-End)

Specifies a grid item’s end position within the grid row by contributing a line, a span, or nothing \(automatic\) to its grid placement, thereby specifying the inline-end edge of its [grid area](https://developer.mozilla.org/en-US/docs/Glossary/grid_areas).

### **Type:** `string | number`

### Conversion

```diff
// CSS
- grid-row-end: auto;

// React Native
+ gridRowEnd: "auto",
```

## [gridRowGap](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-Row-Gap)

Sets the size of the gap \([gutter](https://developer.mozilla.org/en-US/docs/Glossary/gutters)\) between an element's grid rows.

### **Type:** `string | number`

### Conversion

```diff
// CSS
- grid-row-gap: 8;

// React Native
+ gridRowGap: 8,
```

## [gridRowStart](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-Row-Start)

Specifies a grid item’s start position within the grid row by contributing a line, a span, or nothing \(automatic\) to its grid placement, thereby specifying the inline-start edge of its [grid area](https://developer.mozilla.org/en-US/docs/Glossary/grid_areas).

### **Type:** `string | number`

### Conversion

```diff
// CSS
- grid-row-start: todo;

// React Native
+ gridRowStart: "todo",
```

## [gridTemplateColumns](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-Template-Columns)

Defines the line names and track sizing functions of the [grid columns](https://developer.mozilla.org/en-US/docs/Glossary/grid_column).

### **Type:** `string | number | Array<string | number>`

### Conversion

```diff
// CSS
- grid-template-columns: 100px 200px;

// React Native
+ gridTemplateColumns: [100, 200],
```

## [gridTemplateRows](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-Template-Rows)

Defines the line names and track sizing functions of the [grid rows](https://developer.mozilla.org/en-US/docs/Glossary/grid_rows).

### **Type:** `string | number | Array<string | number>`

### Conversion

```diff
// CSS
- grid-template-rows: 40px 4px 40px;

// React Native
+ gridTemplateRows: [40, 4, 40],
```

## [gridTemplateAreas](https://developer.mozilla.org/en-US/docs/Web/CSS/grid-Template-Areas)

Specifies named [grid areas](https://developer.mozilla.org/en-US/docs/Glossary/grid_areas).

### **Type:** `string | 'none'`

### Conversion

```diff
// CSS
- grid-template-areas: "a b c";

// React Native
+ gridTemplateAreas: "a b c",
```

