---
description: >-
  In addition to the default transform style properties provided by React
  Native. React Native for web also provides the following.
---

# Transforms

## The API

### [perspective](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective)

The **`perspective`** style property determines the distance between the z=0 plane and the user in order to give a 3D-positioned element some perspective. Each 3D element with z&gt;0 becomes larger; each 3D-element with z&lt;0 becomes smaller. The strength of the effect is determined by the value of this property.

#### **Type:** `number | string`

#### Conversion

```diff
// CSS
- perspective: 800px;

// React Native
+ perspective: 800,
```

### [perspectiveOrigin](https://developer.mozilla.org/en-US/docs/Web/CSS/perspective-origin)

Determines the position at which the viewer is looking. It is used as the vanishing point by the perspective property.

#### **Type:** `string`

#### Conversion

```diff
// CSS
- perspective-origin: bottom left;

// React Native
+ perspectiveOrigin: "bottom left",
```

### [transformOrigin](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-origin)

The transformation origin is the point around which a transformation is applied. For example, the transformation origin of the rotate\(\) function is the center of rotation. \(This property is applied by first translating the element by the negated value of the property, then applying the element's transform, then translating by the property value.\)

#### **Type:** `string`

#### **Default:** `'50% 50%'`

#### Conversion

```diff
// CSS
- transform-origin: 0% 50%;

// React Native
+ transformOrigin: "0% 50%",
```

### [transformStyle](https://developer.mozilla.org/en-US/docs/Web/CSS/transform-style)

Sets whether children of an element are positioned in the 3D space or are flattened in the plane of the element. If flattened, the element's children will not exist on their own in the 3D-space.

#### **Type:** `'flat' | 'preserve-3d'`

#### Conversion

```diff
// CSS
- transform-style: preserve-3d;

// React Native
+ transformStyle: 'preserve-3d',
```

