# HTML

## Lazy Loading

```html
<!-- prevents loading of images that aren't really needed on the screen immediately -->
<!-- as you scroll down or closer to the image, the image begins to load -->
<img loading="lazy" /> <img loading="eager" />
```

## Refresh Page

```html
<!-- redirects the user to the provided URL in 4 seconds -->
<!-- Set to 0 for an immediate redirect -->
<head>
  <meta http-equiv="refresh" content="4; URL=URL" />
</head>
```

## Picture Element

```html
<!-- add multiple images for different screen sizes -->
<picture>
  <source media="(min-width: 650px)" srcset="medium.png" />
  <source media="(min-width: 450px)" srcset="small.png" />
  <img src="default.png" />
</picture>
```

## Base Element

```html
<!-- for when anchor tags redirect to urls with the same base address -->
<head>
  <base href="http://twitter.com" target="_blank" />
</head>

<body>
  <a href="Elon Musk">Elon Musk</a>
</body>
```

## Datalist

```html
<!-- searchable dropdown list -->
<label for="country">Choose your country</label>
<input list="countries" name="country" id="country" />

<datalist id="countries">
  <option value="Ghana"></option>
  <option value="Japan"></option>
  <option value="England"></option>
</datalist>
```

## Download File

```html
<a href="file.pdf" download="downloaded_file.pdf">download file</a>
```

## Prevent Zooming in

```html
<meta
  name="viewport"
  content="width=device-width, initial-scale=1, user-scalable=0"
/>
```

## Center

```html
<center>i will be centered</center>
```

## Data

```html
<tag data-anything="hello"></tag>
```

## Reset form

```html
<input type="reset" />
```
