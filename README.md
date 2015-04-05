# homeless

> Let' s help the "less" (fortunate) developers

homeless is a library that provides helpful functions for "Less" (Less.js)


## Examples

### each

```
@list: 'a', 'b', 'c';

.each(@list, {.callback(@item) {
  .@{item} {
    item: @item;
  }
}});
```

### for

```
.for(3, {.callback(@i) {
  .for(3, {.callback(@j) {
    .item-@{i}-@{j} {
      i: @i;
      j: @j;
    }
  }});
}});
```

### if

```
.if(isnumber(2), {
    .then(){
        test {
            bool: "pass";
        }
    }
    .else(){
        test {
            bool: "fail";
        }
    }
});
```

### join

```
&{
  @list: a, b, c, d, e, f, g;
  .join(@list);
  .test {
    test: @return;
  }
}
```

### repeat

```
&{
  .repeat('.test', ' ', 3);
  .test {
    test: @return;
  }
}
```
