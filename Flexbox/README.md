# Flexbox

## Introduction to Flexbox

Flexbox is a one-dimensional layout method for arranging items in rows or columns. It is designed to distribute space along a single axis and improve the alignment capabilities of items within a container.

## Key Concepts

### Flex Container

The parent element that holds the flex items. It is defined by setting the `display` property to `flex` or `inline-flex`.

```css
.container {
  display: flex;
}
```

### Flex Items

The direct children of the flex container. These items can be manipulated using various flexbox properties.

### Main Axis and Cross Axis

- **Main Axis**: The primary axis along which flex items are laid out. It can be horizontal or vertical.
- **Cross Axis**: The axis perpendicular to the main axis.

### Properties for the Flex Container

- `flex-direction`: Defines the direction of the main axis (row, row-reverse, column, column-reverse).
- `justify-content`: Aligns flex items along the main axis (flex-start, flex-end, center, space-between, space-around, space-evenly).
- `align-items`: Aligns flex items along the cross axis (flex-start, flex-end, center, baseline, stretch).
- `flex-wrap`: Controls whether flex items should wrap onto multiple lines (nowrap, wrap, wrap-reverse).

### Properties for Flex Items

- `order`: Controls the order of flex items.
- `flex-grow`: Defines the ability of a flex item to grow relative to the rest.
- `flex-shrink`: Defines the ability of a flex item to shrink relative to the rest.
- `flex-basis`: Defines the default size of a flex item before the remaining space is distributed.
- `align-self`: Allows the default alignment to be overridden for individual flex items.

## Visual Examples

### Basic Flexbox Layout

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.item {
  background-color: lightblue;
  padding: 10px;
  margin: 5px;
}
```

### Flex Direction

```css
.container {
  display: flex;
  flex-direction: column;
}
```

### Justify Content

```css
.container {
  display: flex;
  justify-content: space-around;
}
```

### Align Items

```css
.container {
  display: flex;
  align-items: flex-end;
}
```

Flexbox is a powerful tool for creating responsive and flexible layouts. By mastering its properties and concepts, you can build complex designs with ease.
