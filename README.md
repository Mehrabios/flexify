# Flexify
Flexify is a lightweight CSS library based on flexbox used for page layout.

## Why To Use
CSS isn't hard to work with, but it's painful. Creating a layout system is hard, but once you have it, it really makes your project easier. CSS frameworks like Bootstrap give us this layout system, but they are too big and not suitable for people who just want to use "plain CSS". So I created this little "library" for myself and others like me to use. This library is customizable with SCSS and CSS custom properties, and I will add new features to it in the future.

## Table Of Content 
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)

## Installation
Installing with NPM:

```bash
npm i flexify
```

Using CDN:

```html
<link rel="stylesheet" href="https://www.jsdelivr.com/package/npm/flexify/css/flexify.min.css">
```

## Usage
`.continer` class will make a responsive container, like bootstrap:

```html
<div class="continer"></div>
```

`.row` class will make a row, inside of the `row` element you can use columns:

```html
<div class="row">
  <div class="col-auto"></div>
</div>
```

`.col-#breakpoint-#size-b#column` class will create a responsive column.

- #breakpoint refers to breakpoints, it means that what size is used in diffrent devices. it uses bootstrap breakpoints.  possible values are `sm`, `md`, `lg`

- #size refers to the size of a column, for example in a 12-column based layout system, possible values ​​are numbers between 1 and 13.

- #column refres to what kind of layout system do you want to use, possible values are `6`, `8`, `12`.

Note: In Bootstrap, you can only use 12 column based layout system, but in flexify you can use 6, 8 or even 12 column based layout system.

```html
<!-- 12 column based layout system -->

<div class="row">
  <div class="col-12-b12 col-md-2-b12"></div>
  <div class="col-12-b12 col-md-4-b12"></div>
  <div class="col-12-b12 col-md-3-b12"></div>
  <div class="col-12-b12 col-md-3-b12"></div>
  <div class="col-auto"></div>
</div>

<!-- 8 based layout system -->

<div class="row">
  <div class="col-8-b8 col-md-2-b8"></div>
  <div class="col-8-b8 col-md-3-b8"></div>
  <div class="col-8-b8 col-md-1-b8"></div>
  <div class="col-8-b8 col-md-2-b8"></div>
  <div class="col-auto"></div>
</div>

<!-- 6 based layout system -->

<div class="row">
  <div class="col-6-b6 col-lg-2-b6"></div>
  <div class="col-6-b6 col-lg-2-b6"></div>
  <div class="col-6-b6 col-lg-2-b6"></div>
  <div class="col-auto"></div>
</div>
```

## License
This project is licensed under the [MIT License](LICENSE).
