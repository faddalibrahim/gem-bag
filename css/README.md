# CSS GEMS

## Selectors

```
~
+
>
```

```css
scroll-bahavior: smooth;

used with <a href="footer"/ > <footer id="footer"/ > also with :target {
}
```

```css
input {
  accent-color: red;
}
```

```css
tag {
  user-select: none;
}
```

```css
tag {
  pointer-events: none;
}
```

```css
tag {
  width: fill-available | min-content | max-content | fit-content;
}
```

## attr

```html
<div data="hello">hello</div>
```

```css
div:after {
  content: attr(data);
}
```

# Form Elements

```css
checkbox:checked + label {
  text-decoration: strikethrough;
}

radio:checked + label {
  color: red;
}

input:focus + label {
  color: red;
}

form div:focus-within header {
  background-color: orange;
}

button:active {
}

button:focus {
}
```
