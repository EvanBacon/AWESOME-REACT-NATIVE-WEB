---
description: >-
  Because RNWeb doesn't support the React Native LayoutAnimation API we need to
  use other methods for animating our components around the screen. A good
  alternative is the CSS Transitions API.
---

# Transitions

## What can it do?

CSS Transitions enable us to create implicit transitions similar to techniques like "magic move". You can define how you want the transition to take place and the final position, but the browser is responsible for interpolating the values.

## The API

### transitionDelay

The duration or durations an animation will wait before starting or proceeding to interpolate to the next value.

#### **Type:** `string | string[]`

```text
transitionDelay: "200ms"
transitionDelay: ["1s", "300ms"]
```

### transitionDuration

Durations of the transitions after the delay has finished. Durations are strings that can be prefixed with either "s" for seconds or "ms" for milliseconds.

#### **Type:** `string | string[]`

**Default:** `"0s"`

```text
transitionDuration: "200ms"
transitionDuration: ["1s", "300ms"]
```

### transitionProperty

Define the name or names of the properties that should be controlled by the transition effect. The transition will begin whenever one of the specified properties change.

#### **Type:** `string | string[]`

**Values:** `"none" | "all" | property`

**Default:** `"all"`

```text
transitionProperty: "all"
transitionProperty: ["width", "height"]
```

### transitionTimingFunction

This value denotes the speed curve of the transition effect. Learn more about [CSS Transition Timing Functions](https://www.w3schools.com/cssref/css3_pr_transition-timing-function.asp).

#### **Type:** `string | string[]`

**Values:** `"linear" | "ease" | "ease-in" | "ease-out" | "ease-in-out" | "step-start" | "step-end" | "steps(int,start|end)" | "cubic-bezier(n,n,n,n)"`

```text
transitionTimingFunction: "linear"
transitionTimingFunction: ["ease", "ease-out"]
```

