# grid

Mastering the basics of css grid

### Shortcuts

To create a starting html document

```
!+enter
```

To add 20 div items to a grid:

```
<div class="grid">
.item.item-${$$}*20 + enter
</div>
```

### Responsive

To make the columns in grid responsive:

```
.grid {
  display: grid;
  grid-template-columns: auto auto;
}
```

You can change the size of the columns and the number of columns(4col) It distributes the items into those columns:

```
.grid {
  display: grid;
  grid-template-columns: 200px 40% 20% 15%;
}
```

Or you can use the fractions unit to devide the grid into columns ex:

- grid-template-columns: 1fr 2fr 4fr
  - The above means the second column to be twice as big as the first one and the third one to be 2 times as big as the second one
    Or you can have many columns by adding repeat ex:
  - grid-template-colums: repeat(12, 100px) - The above means you get 12 columns of 100px each
    To alternate sizes of columns:
- grid-template-columns: repeat(6, 100px 200px)
  - The above will make 12 columns: 6 measuring 100px and 6 measuring 200px alternating
    To make 6 columns same size:
- grid-template-colums: repeat(6, auto)
