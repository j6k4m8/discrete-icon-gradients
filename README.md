# Discrete-Icon-Gradient
A LESS mixin collection that allows you to show a partially-filled texticon.

Perfect for when you have an icon of signal-bars or such and want to fill some but not all of them. Allows for partially-transparent 'missing' bars, your own fallbacks, etc. Should be pretty cross-compatible, but no promises.


##Usage
Let's say we want to modify this icon to be more colorful:

Simply say, 
```
.discrete-gradient(red, blue, 30%);
```
which translates to:
```
.glyphicons-th-list {
    background: linear-gradient(to right, red 0%,red 29%,blue 30%,blue 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}
```


Here, we fill 33% of the icon (the left 33%) with red, and the rest of the icon with a red-transparent color.

## Another Example
```
<i class="example0">&amp;</i>
```

```
.example0 {
    .discrete-gradient(blue, fade(blue, 50%), 50%);
}
```

Which results in: 

![image](example0.png)
