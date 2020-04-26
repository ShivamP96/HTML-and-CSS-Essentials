# Grid Box Notes
A simple breakdown of some grid garden


## Columns

``` css
#water {
  grid-column-start: 3;
}
 This means that the water will start at the 3rd vertical grid line, Which is another way of saying the 3rd vertical border from the left of the grid. 
```

![Basic Layout](./pictures/gridGardenLayout.png)

You can see above how water started from the 3rd vertical line

``` css
#water {
grid-column-start: 1;
grid-column-end: 4;

}
When grid-column-start is used alone, the grid item by default will span exactly one column. However, you can expand the item across multiple columns by adding the grid-column-end property

grid-column-end will end at the vertical line that you set it to
```

![Using grid-column-end](./pictures/gridGardenEnd.png)

```css
#water {
  grid-column-start: 5;
  grid-column-end: 2;
}

When using start and end, the end value doesn't have to be greater than the start value

```

#### You can also do negatives

If you want to count grid lines from the right instead of the