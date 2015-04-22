# ExpandSelect.js #

An `ExpandSelect()` javascript function that emulates mouse clicking on the html `<select>` element.

## Download ##

Version 1.00: [ExpandSelect\_1.00.js](http://expandselect.googlecode.com/files/ExpandSelect_1.00.js) (4 KB)

Or view the file in your browser: [browse/ExpandSelect.js](http://code.google.com/p/expandselect/source/browse/ExpandSelect.js)

<a href='https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=9BNEBWTQDAVLU'><img src='https://www.paypalobjects.com/en_US/GB/i/btn/btn_donateCC_LG.gif' /></a>

Thanks to the individuals that have donated: Lars Bentzen, Edoardo De Zorzi.

## How it works? ##

Browsers do not allow expanding `<select>` in pure javascript, that control can be expanded only by directly clicking on it using the mouse. The "select.click()" won't work. But there is a solution. We imitate expanded `<select>` control by creating another select with multiple options being displayed at once, this can be done by setting the "size" parameter. That multi select will be positioned absolutely over the old single-option select control, and the old one will be hidden using style's visibility. That way the layout is kept the same, and the new control is displayed seamlessly. The new control looks only little differently, but that shouldn't be a problem, see it for yourself in screenshots below.

## Compatibility ##

All major browsers have been tested: Chrome, Firefox, Opera, Internet Explorer.

## How to use ##

Call function ExpandSelect() on your `<select>` element, you can provide the element itself or its identifier, see the code:

```js

ExpandSelect(myselect);
// or:
ExpandSelect("myselect_id");```

## Screenshots ##

On the left you see `<select>` that is mouse clicked, on the right you see the emulation using ExpandSelect() function.

<table border='0'>

<tr>
<td align='center'><b>Mouse clicking</b> with few options:</td>
<td>-----</td>
<td align='center'><b>Emulating click</b> with few options:</td>
</tr>

<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>

<tr>
<td><img src='https://expandselect.googlecode.com/hg/mouseclick_fewoptions.jpg' /></td>
<td></td>
<td><img src='https://expandselect.googlecode.com/hg/emulateclick_fewoptions.jpg' /></td>
</tr>

<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>

<tr>
<td align='center'><b>Mouse clicking</b> with many options:</td>
<td>-----</td>
<td align='center'><b>Emulating click</b> with many options:</td>
</tr>

<tr>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
</tr>

<tr>
<td><img src='https://expandselect.googlecode.com/hg/mouseclick_manyoptions.jpg' /></td>
<td></td>
<td><img src='https://expandselect.googlecode.com/hg/emulateclick_manyoptions.jpg' /></td>
</tr>

</table>

## Copyright and license ##

Copyright (c) Czarek Tomczak. All rights reserved.

Licensed under New BSD License (free for any use, read more at http://www.opensource.org/licenses/bsd-license.php)