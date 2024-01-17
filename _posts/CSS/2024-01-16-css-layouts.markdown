---
layout: post
title: Flexbox and CSS Grid
author: Psylar87
comments: True
---

<hr>

<h3><strong>Flexbox (Flexible Box):</strong></h3>

<b>Purpose:</b>  Flexbox is designed for one-dimensional layouts, either in a row or a column. It's particularly useful for laying out items within a container and distributing space along a single axis. 

<p>
<b>Container Properties:</b> 
</p>
```display: flex;``` This property is applied to the container, turning it into a flex container.
```flex-direction: row|column;``` Specifies the main axis direction (row or column).
```justify-content: flex-start|flex-end|center|space-between|space-around;``` Aligns items along the main axis.
```align-items: stretch|flex-start|flex-end|center|baseline;``` Aligns items along the cross axis.

<p>
<b>Item Properties:</b>
</p>
```order:<integer>;``` Specifies the order of the flex items.
```flex-grow: <number>;``` Defines the ability for a flex item to grow.
```flex-shrink: <number>;``` Defines the ability for a flex item to shrink.
```flex-basis: <length|auto>;``` Specifies the initial size of a flex item.

<b>Example:</b>

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```
<hr>
<br>

<h3><strong>CSS Grid:</strong></h3>

<b>Purpose:</b> CSS Grid is a two-dimensional layout system that allows you to create grid-based layouts. It's ideal for both rows and columns and offers precise control over the placement and sizing of items within the grid.

<p>
<b>Container Properties:</b>
</p>
```display: grid;``` This property is applied to the container, turning it into a grid container.
```grid-template-rows: <track-size>;``` Defines the size of each row in the grid.
```grid-template-columns: <track-size>;``` Defines the size of each column in the grid.
```grid-gap: <row-gap> <column-gap>;``` Sets the gap size between rows and columns.

<p>
<b>Item Properties:</b>
</p>
```grid-row: <start-line> / <end-line>;``` Specifies the size and location of an item in terms of rows.
```grid-column: <start-line> / <end-line>;``` Specifies the size and location of an item in terms of columns.
```grid-area: <row-start> / <column-start> / <row-end> / <column-end>;``` A shorthand for specifying both row and column placements.

<b>Example:</b>

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
}
```

Both Flexbox and CSS Grid are widely supported in modern browsers, and they can be used together to create sophisticated layouts. The choice between them often depends on the specific requirements of your layout. Flexbox is great for simpler, one-dimensional layouts, while CSS Grid excels at handling more complex, two-dimensional layouts.

<br>
<p>
<strong>Please Note: I am not an expert and this is more or less a way for me to help cement the basics of this concept in my own mind. If this is of any value to you, that's just an added bonus.</strong>
</p>

<hr>