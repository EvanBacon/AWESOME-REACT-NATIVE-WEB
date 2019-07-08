---
description: >-
  React Native for web adds the following features to the React Native <View />
  element.
---

# View

The props shown here come from the `ViewPropTypes` object. Primitives that extend `ViewPropTypes` also have access to these custom props for example: `<Image /> <Text /> <TextInput /> <ScrollView />` 

## Props

### [draggable](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/draggable)

Can the user drag the element around. If this attribute is not set, its default value is auto, which means drag behavior is the default browser behavior: only text selections, images, and links can be dragged.

#### **Type:** `boolean`

#### **Default:** `true`

#### Conversion

```diff
// HTML
- <div draggable="true"></div>

// React Native
+ <View draggable />
```

### [onContextMenu](https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers/oncontextmenu)

The `onContextMenu` method is invoked when the user attempts to open a context menu. This event is typically triggered by clicking the **right mouse button**, or by pressing the context menu key. In the latter case, the context menu is displayed at the bottom left of the focused element, unless the element is a tree, in which case the context menu is displayed at the bottom left of the current row.

Any right-click event that is not disabled \(by calling the event's `preventDefault()` method\) will result in the method being invoked.

#### **Type:** `Function`

#### Conversion

```diff
// HTML & JavaScript
- <div id="noContextMenu"></div>

- let element = document.getElementById('noContextMenu');
-
- element.addEventListener('contextmenu', e => {
- });

// React Native
+ <View onContextMenu={(e) => {}} />
```

### [itemID](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/itemid)

Provides microdata in the form of a unique, global identifier of an item. An `itemID` attribute can only be specified for an element that has both `itemScope` and `itemType` attributes. Also, `itemID` can only be specified on elements that possess an itemscope attribute whose corresponding `itemType` refers to or defines a vocabulary that supports global identifiers.

The exact meaning of an `itemType`'s global identifier is provided by the definition of that identifier within the specified vocabulary. The vocabulary defines whether several items with the same global identifier can coexist and, if so, how items with the same identifier are handled.

#### **Type:** `string`

#### Conversion

```diff
// HTML
- <div itemid=""></div>

// React Native
+ <View itemID="" />
```

### [itemRef](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/itemref)

Properties that are not descendants of an element with the `itemScope` attribute can be associated with an item using the global attribute `itemRef`.

`itemRef` provides a list of element IDs \(not `itemID`s\) elsewhere in the document, with additional properties.

The `itemRef` attribute can only be specified on elements that have an `itemScope` attribute specified.

#### **Type:** `string`

#### Conversion

```diff
// HTML
- <div itemref=""></div>

// React Native
+ <View itemRef="" />
```

### [itemProp](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/itemprop)

The `itemProp` global attribute is used to add properties to an item. Every HTML \(Not JSX\) element can have an `itemProp` attribute specified, and an `itemProp` consists of a name-value pair. Each name-value pair is called a **property**, and a group of one or more properties forms an item. Property values are either a string or a URL and can be associated with a very wide range of elements including `<WebView />`, `<Image />`, and `<Expo.Video />`.

#### **Type:** `string`

#### Conversion

```diff
// HTML
- <div itemprop="coder"></div>

// React Native
+ <View itemProp="coder" />
```

### [itemScope](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/itemscope)

`itemScope` is a `boolean` global attribute that defines the scope of associated metadata. Specifying the `itemScope` attribute for an element creates a new item, which results in a number of name-value pairs that are associated with the element. A related attribute, `itemType`, is used to specify the valid URL of a vocabulary \(such as [schema.org](https://schema.org/)\) that describes the item and its properties context.

Every primitive React Native web element may have an `itemScope` attribute specified. An `itemScope` element that does not have an associated `itemType` must have an associated `itemRef`.

#### **Type:** `boolean`

#### Conversion

```diff
// HTML
- <div itemscope itemtype="http://schema.org/Movie">
-   <h1 itemprop="name">Avatar</h1>
-   <span>Director: <span itemprop="director">James Cameron</span> (born August 16, 1954)</span>
-   <span itemprop="genre">Science fiction</span>
-   <a href="https://youtu.be/0AY1XIkX7bY" itemprop="trailer">Trailer</a>
- </div>

// React Native
+ <View itemScope itemType="http://schema.org/Movie">
+   <Text accessibilityRole="header" itemProp="name">Avatar</Text>
+   <Text>Director: <Text itemProp="director">James Cameron</Text> (born August 16, 1954)</Text>
+   <Text itemProp="genre">Science fiction</Text>
+   <Text accessibilityRole="link" href="https://youtu.be/0AY1XIkX7bY" itemProp="trailer">Trailer</Text>
+ </View>
```

### [itemType](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/itemtype)

The global attribute `itemType` specifies the URL of the vocabulary that will be used to define `itemProp`'s \(item properties\) in the data structure. `itemScope` is used to set the scope of where in the data structure the vocabulary set by `itemType` will be active.

Google and other major search engines support the [schema.org](http://schema.org/) vocabulary for structured data. This vocabulary defines a standard set of type names and property names. For example, [`MusicEvent`](http://schema.org/MusicEvent) indicates a concert performance, with [`startDate`](http://schema.org/startDate) and [`location`](http://schema.org/location) properties specifying the concert's key details. In this case, [`MusicEvent`](http://schema.org/MusicEvent) would be the URL used by `itemType`, with [`startDate`](http://schema.org/startDate) and [`location`](http://schema.org/location) as `itemProp`'s which MusicEvent defines.

#### **Type:** `string`

#### Conversion

```diff
// HTML
- <div itemscope itemtype="http://schema.org/Product">
-  <span itemprop="brand">Supreme</span>
-  <span itemprop="name">Brick</span>
- </div>

// React Native
+ <View itemScope itemType="http://schema.org/Product">
+  <Text itemProp="brand">Supreme</Text>
+  <Text itemProp="name">Brick</Text>
+ </View>
```

