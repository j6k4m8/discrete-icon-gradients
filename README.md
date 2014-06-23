# Discrete-Icon-Gradient
A LESS mixin collection that allows you to show a partially-filled texticon.

Perfect for when you have an icon of signal-bars or such and want to fill some but not all of them. Allows for partially-transparent 'missing' bars, your own fallbacks, etc. Should be pretty cross-compatible, but no promises.


##Usage
```
<div class="two-bars phone-signal-icon"></div>
```

```
.two-bars {
    .discrete-gradient(red, fade(red, 30%), 33%);
}
```

Here, we fill 33% of the icon (the left 33%) with red, and the rest of the icon with a red-transparent color.

## Another Example
```
<i class="example0">&</i>
```

```
.example0 {
    .discrete-gradient(blue, fade(blue, 50%), 50%);
}
```

