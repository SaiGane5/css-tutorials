# CSS Grid

## Key Concepts

### Grid Container

A grid container is an element on which `display: grid` is applied. It’s the direct parent of all the grid items.

```css
.container {
  display: grid;
}
```

### Grid Item

A grid item is a direct child of the grid container.

### Grid Lines

Grid lines are the dividing lines that make up the structure of the grid. They can be either vertical or horizontal.

### Grid Tracks

Grid tracks are the space between two grid lines. They can be either rows or columns.

### Grid Cell

A grid cell is the space between four grid lines. It’s a single “unit” of the grid.

### Grid Area

A grid area is a rectangular area that consists of one or more grid cells.

## Visualizations

### Grid Container and Items

```html
<div class="container">
  <div class="item">1</div>
  <div class="item">2</div>
  <div class="item">3</div>
</div>
```

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 10px;
}

.item {
  background-color: lightblue;
  padding: 20px;
  text-align: center;
}
```

### Grid Lines and Tracks

```css
.container {
  display: grid;
  grid-template-columns: 100px 200px;
  grid-template-rows: 100px 200px;
}
```

### Grid Area

```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar content"
    "footer footer";
}

.header {
  grid-area: header;
}

.sidebar {
  grid-area: sidebar;
}

.content {
  grid-area: content;
}

.footer {
  grid-area: footer;
}
```

```html
<div class="container">
  <div class="header">Header</div>
  <div class="sidebar">Sidebar</div>
  <div class="content">Content</div>
  <div class="footer">Footer</div>
</div>
```
