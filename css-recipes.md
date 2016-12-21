# Cross Browser Opacity

```css
.transparent_class {
  /* IE 8 */
  -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=50)";

  /* IE 5-7 */
  filter: alpha(opacity=50);

  /* Netscape */
  -moz-opacity: 0.5;

  /* Safari 1.x */
  -khtml-opacity: 0.5;

  /* Good browsers */
  opacity: 0.5;
}
```
From [CSS Tricks](https://css-tricks.com/snippets/css/cross-browser-opacity/)

# Fixed centred header with margins

```css
.class-name {
    position: fixed;
    /* center the element */
    right: 0;
    left: 0;
    margin-right: auto;
    margin-left: auto;
    /* give it dimensions */
    min-height: 10em;
    width: 90%;
}
```

Another option
```css
.site-header {
    position: fixed;
    left: 50%;
    margin-left: -570px;
    width: 1140px;
}
```

From [Sitepoint Forums](https://www.sitepoint.com/community/t/how-to-center-a-position-fixed-header/37232/2)

#Center a column using Bootstrap

[Good explanation on StackOverflow with examples](http://stackoverflow.com/a/20358578/2302700)
