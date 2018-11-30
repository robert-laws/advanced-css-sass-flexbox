# Flexbox - learning form the Advanced CSS and Sass course from Udemy by Jonas Schmedtmann

Following along with the course content - to build up flexbox skills and knowledge.

## Core Concepts

Flex container

```css
/* Invoke flexbox behavior */
.container {
  display: flex;
}
```

Main axis - left-to-right axis when flex-direction is row

Cross axis - top-to-bottom axis when flex-direction is row

Flex items - items within the flex container

## Flex Container Properties

Flex direction - designation of main axis and it's direction. `flex-direction: row | row-reverse | column | column-reverse` Default behavior is row.

Flex wrap - flex items will wrap if there's not enough space.

Justify content - designates how items will align along the *main-axis*. `justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly`

Align items - designates how items will align along the *cross-axis*. `align-items: stretch | flex-start | flex-end | center | baseline`

Align content - designates how items will align along the cross-axis when there's more than row of flex items. `align-content: stretch | flex-start | flex-end | center | space-between | space-around`

```css
.container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: center;
}
```

## Flex Items Properties

Align self - applies alignment to one item, allowing it to align differently than set in the align-items property setting. `align-self: auto | stretch | flex-start | flex-end | center | baseline`

Order - defines order where one particular item should appear in relation to others. `order: 0 | <integer>`

Flex grow - defines how a flex item will grow in relation to other items in the flex container `flex-grow: 0 | <integer>`

Flex shrink - defines how a flex item will shrink in relation to other items in the flex container `flex-shrink: 1 | <integer>`

Flex basis - defines a flex item base width. `flex-basis: auto | <length>`

Shorthand for flex-grow, flex-shrink, and flex-basis: `flex: 0 1 auto`