# HTML

```html
<!-- prevents loading of images that aren't really needed on the screen immediately -->
<!-- as you scroll down or closer to the image, the image begins to load -->
<img loading="lazy" /> <img loading="eager" />
```

```html
<!-- redirects the user to the provided URL in 4 seconds -->
<!-- Set to 0 for an immediate redirect -->
<head>
  <meta http-equiv="refresh" content="4; URL=URL" />
</head>
```

```html
<!-- add multiple images for different screen sizes -->
<picture>
  <source media="(min-width: 650px)" srcset="medium.png" />
  <source media="(min-width: 450px)" srcset="small.png" />
  <img src="default.png" />
</picture>
```

```html
<!-- for when anchor tags redirect to urls with the same base address -->
<head>
  <base href="http://twitter.com" target="_blank" />
</head>

<body>
  <a href="Elon Musk">Elon Musk</a>
</body>
```

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

```html
<a href="file.pdf" download="downloaded_file.pdf">download file</a>
```
