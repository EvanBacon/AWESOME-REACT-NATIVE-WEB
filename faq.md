# FAQ

### The name "React Native for web" is scary

A universal issue with React Native for web is the name. If you're familiar with **ReactDOM** you may know that the **JSX** elements `div`, `span`, `img` aren't actually **HTML**, rather a set of components that bind to DOM elements. At its core RNWeb is just a set of primitives that bind components like `View`, `Image`, or `Text` to DOM elements like `div`, `img`, and `span`. These primitives provide the foundation for creating universal applications. 

### What kinda websites does this build?

When you bundle a React Native for web project with Webpack \(or `expo build:web`\) you are creating a static react website that can be hosted anywhere. Generally because you made a universal application, your final product will come out feeling more like a web _app_ then a traditional website. This is because you'll more than likely be using complex native APIs like Camera, ImagePicker, Gesture Handler, or MapView in the browser.

### Should I use Expo or React Native for web?

Expo provides a set of tools for building high-quality applications \(with React Native\). The goal of Expo for web is to create a seamless experience when building on whatever platform you have available. Expo provides universal bindings for things like Camera, Location, Gestures that work together on whatever platform Expo supports. Expo also smooths over a lot of the issues regarding bundling your app and ensuring it works the same in Webpack \(React\) and Metro \(React Native\).

