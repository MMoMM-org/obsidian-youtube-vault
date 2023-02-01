test:: hello world

#recording

## People

[[@Tom]]
[[@Marry]]

## Projects

[[401 Project 1]]
[[402 Project 2]]


## Custom Styling

Show the status property value while hovering on link

```css
.data-link-icon-after[data-link-status]:hover::after{
    content: " ► "attr(data-link-status)
}
```

