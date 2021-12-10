# ColorNames
this is a collection of colors codes and their common name. All data is collectd combined from
https://xkcd.com/color/rgb.txt which is CC0 and from an RAL data set which should also be CC0.

The data is structured as following

| Index | Field Name | Description                           |
|-------|------------|---------------------------------------|
| 0     | Name       | name of the color                     |
| 1     | Hex        | hex code of the color prefixed with # |
| 2     | R          | red in RGB                            |
| 3     | G          | green in RGB                          |
| 4     | B          | blue in RGB                           |
| 5     | L          | lightness (L) part in CIELAB          |
| 6     | a          | a-axis (a) part in CIELAB             |
| 7     | b          | b-axis (b) part in CIELAB             |

The inclusion of the lab CIELAB values is meant to make approximation of
colors easier since calculating delta e via [CIEDE2000](http://www2.ece.rochester.edu/~gsharma/ciede2000/ciede2000noteCRNA.pdf)
is relatively straight forward and precise.