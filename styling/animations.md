---
description: >-
  Because RNWeb doesn't support the React Native LayoutAnimation API we need to
  use other methods for animating our components around the screen. A good
  alternative is the CSS Transitions API.
---

# Animations

## What can it do?

With CSS Animations in React Native \(for web\) we can create awesome effects with the components on the screen. When you define \(at minimum\) a component's `animationDuration` style property, then any state change that effects that component's style will create an implicit interpolation between the old value and the new one.

## The API

### [animationDelay](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-delay)

The duration to wait before executing the transition associated with a new style value. The value is defined as a `string` with the suffix "s" for seconds or "ms" milliseconds.

#### **Type:** `string | string[]`

#### **Default:** `'0s'`

#### Conversion

```diff
// CSS
- animation-delay: 650ms;

// React Native
+ animationDelay: "650ms",
```

### [animationDirection](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-direction)

The direction value dictates if an animation should be played forwards, backwards or in alternate cycles.

#### **Type:** `string | string[]`

#### **Default:** `'normal'`

#### **Values:** `'alternate' | 'alternate-reverse' | 'normal' | 'reverse'`

#### Conversion

```diff
// CSS
- animation-direction: alternate-reverse;

// React Native
+ animationDirection: "alternate-reverse",
```

### [animationDuration](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-duration)

The duration or durations of the animations after the `animationDelay` has finished. The value is defined as a `string` with the suffix "s" for seconds or "ms" milliseconds.

#### **Type:** `string | string[]`

#### **Default:** `'0s'`

#### Conversion

```diff
// CSS
- animation-duration: 10s;

// React Native
+ animationDuration: "10s",
```

### [animationFillMode](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-fill-mode)

The `animationFillMode` CSS property sets how a CSS animation applies styles to its target before and after its execution.

#### **Type:** `string | string[]`

#### **Default:** `'forwards'`

#### **Values:** `'none' | 'forwards' | 'backwards' | 'both'`

#### Conversion

```diff
// CSS
- animation-fill-mode: none;

// React Native
+ animationFillMode: "none",
```

### [animationIterationCount](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-iteration-count)

The `animationIterationCount` CSS property sets the number of times an animation cycle should be played before stopping.

If multiple values are specified, each time the animation is played the next value in the list is used, cycling back to the first value after the last one is used.

#### **Type:** `number | 'infinite' | Array<number, 'infinite'>`

#### **Default:** `1`

#### **Values:** `<number> | 'infinite'`

#### Conversion

```diff
// CSS
- animation-iteration-count: 2;

// React Native
+ animationIterationCount: 2,
```

### [animationKeyframes](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-key-frames)

Used to control the intermediate steps in an animation sequence by defining styles for keyframes \(or waypoints\) along the animation sequence. This gives more control over the intermediate steps of the animation sequence than transitions.

#### **Type:** `string | Object | Array<string, Object>`

#### Conversion

```diff
// CSS

- @keyframes demo {
-   0% { backgroundColor: "blue"; }
-   100% { backgroundColor: "red"; }
- }

- animation-name: demo;

// React Native

+ const demo = {
+   '0%': { backgroundColor: "blue" },
+   '100%': { backgroundColor: "red" },
+ }

+ animationKeyframes: demo,
```

### [animationPlayState](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-play-state)

The `animationPlayState` CSS property sets whether an animation is running or paused.

Resuming a paused animation will start the animation from where it left off at the time it was paused, rather than starting over from the beginning of the animation sequence.

#### **Type:** `string | string[]`

#### **Default:** `'running'`

#### **Values:** `'paused' | 'running'`

#### Conversion

```diff
// CSS
- animation-play-state: running;

// React Native
+ animationPlayState: "running",
```

### [animationTimingFunction](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-timing-function)

The `animationTimingFunction` CSS property sets how an animation progresses through the duration of each cycle.

#### **Type:** `string | string[]`

#### **Default:** `'normal'`

**Values:** `"linear" | "ease" | "ease-in" | "ease-out" | "ease-in-out" | "step-start" | "step-end" | "steps(int,start|end)" | "cubic-bezier(n,n,n,n)"`

#### Conversion

```diff
// CSS
- animation-timing-function: ease-in;

// React Native
+ animationTimingFunction: "ease-in",
```

