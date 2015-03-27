# [Sass Font Face Mixins! The Cross-Browser Font Face Sass Mixin]

By: [Sahil Malik] [@sahilmalik1990](https://twitter.com/hashtag/sahilmalik5)

Font Face Sass Mixin to create font face for all browsers including IE.

Font Face Sass Mixin File to be `@imported` and `@included` as you need.

The purpose of this directory is to facilitate the use of Font Face on different browsers avoiding HARD TO READ and NEVER ENDING css files.

From: http://compass-style.org/reference/compass/css3/font_face/
http://www.fontsquirrel.com/tools/webfont-generator


'font-face($name, $font-file-name, $font-files, $eot, $font-weight,$font-style)
---------------------------------------------------------------
 
Cross-browser support for @font-face. Supports IE, Gecko, Webkit, Opera.
 
## Examples and Instructions 
$name is required, name of your font like "Ostwald".
$font-file-name is required using font-files('relative/location', 'format'). for best results use this order: woff, opentype/truetype, svg, It defines the name of your font file like oswald.bold-webfont without extension(.woff,.svg,.ttf etc...).
$font-files is used to generate all the url's for the fonts having different extension.
$eot is required by IE, and is a relative location of the eot file using "#".
$weight shows if the font is bold, defaults to normal
$style defaults to normal, might be also italic. Order of the includes matters, and it is: normal, bold, italic, bold+italic

## Include Fonyt Face Sass Mixin in your project 
    sass
   // Import the mixins
   @import "font-face.scss"

   // Call Mixins
   @include font-face ('oswaldbold','oswald.bold-webfont','#oswaldbold');
   @include font-face ('oswaldregular','oswald.regular-webfont','#oswaldregular');
   

## Licence

Copyright &copy; 2015 Sahil Malik

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.   