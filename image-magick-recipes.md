ImageMagick Recipes
========================

# How to add suffix to output image file names

You need to use `-set` parameter to prepare your custom suffix string and 	`+adjoin` parameter to generate multiple output images.
For example, following command resizes all JPEG images with adding `-large` prefix to output images.

```shell
convert *.jpg -resize 1024 -set filename:f '%t-large.%e' +adjoin '%[filename:f]'
```

# How to resize images with fixed height

You can use `x[hieght_value]` as argument of `-resize` parameter

```shell
convert input.jpg -resize x400 output.jpg
```
