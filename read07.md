# CSS Colors
There are six ways to declare CSS colors:
•	Hexadecimal notation
•	RGB
•	RGBA
•	HSL
•	HSLA
•	Color keywords

Hexadecimal
![](https://www.webfx.com/blog/images/assets/cdn.sixrevisions.com/0481-02-hex-notation-blue.png);

xample
div {
 background-color: #000000;
}

# RGB Color Values

![dd](https://i.pinimg.com/originals/48/35/12/483512cace451ffcdaed62d03beedcec.png);



Most of you have probably heard about CMYK values for print design. RGB, which stands for red, green, and blue is the color model that monitors use. Since in web design we're primarily concerned with what web pages look like on screens, RGB is the color model we use.

    RGB colors have three values that represent: red, green, and blue
    Each value can be a number between 0 and 255 or a percentage from 0 to 100%
    A value of 0 means none of that color is being used
    A value of 255 or 100% means all of that color is being used
    A 0 for all three color values will be black
    A 255 or 100% for all three color values will be white

The CSS syntax for using RGB colors is a little different than we've seen before. In the example below, we are styling:

    A black paragraph
    A white h1
    A purple unordered list

p { color: rgb(0, 0, 0); }              /* black */
h1 { color: rgb(255, 255, 255); }       /* white */
ul { color: rgb(128, 80, 200); }        /* purple */

/* Percentages work too */
h1 { color: rgb(100%, 100%, 100%); }    /* white */



RGBA is all the rage.

Seriously though, it's just like RGB, except with the addition of a fourth value: the alpha channel.

The alpha value represents the level of transparency that the rgb color should have. It can be a value from 0 to 1 or a percentage from 0 to 100%. Note that you must specify RGBA instead of RGB.

Grid Example

This grid shows varying saturation and lightness together

HSLA Color Values

HSLA color values are an extension of HSL color values with an Alpha channel - which specifies the opacity for a color.

An HSLA color value is specified with:

hsla(hue, saturation, lightness, alpha)

The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (not transparent at all):

Experiment by mixing the HSLA values below:

hsla(0, 100%, 50%, 0.5 )




> by kefah