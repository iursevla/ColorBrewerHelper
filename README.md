# ColorBrewerHelper
Static helper class to access ColorBrewer color schemes.

# Example usage:

### 1.ColorBrewer.getColors('Spectral', 7);
Result:
```
[ [ '213', '62', '79' ],
  [ '252', '141', '89' ],
  [ '254', '224', '139' ],
  [ '255', '255', '191' ],
  [ '230', '245', '152' ],
  [ '153', '213', '148' ],
  [ '50', '136', '189' ] ]
  ``` 
  This is an array of colors for the Spectral color scheme with 7 classes.

### 2.ColorBrewer.byName('Spectral');
Result:
```
{ '3': [ 'rgb(252,141,89)', 'rgb(255,255,191)', 'rgb(153,213,148)' ],
  '4':
   [ 'rgb(215,25,28)',
     'rgb(253,174,97)',
     'rgb(171,221,164)',
     'rgb(43,131,186)' ],
  '5': [...],
  '6'...
}
```
This is the complete Spectral color scheme. With this object you can do something line obj[7] to get the color for this object with 7 classes (Which is the same as example 1, excepth instead of an array of number you now have an array of rgb(...)).

### 3.ColorBrewer.byNumber(3);
Result:
```
{ 
    Diverging:{
     Spectral: [ 'rgb(252,141,89)', 'rgb(255,255,191)', 'rgb(153,213,148)' ],
     RdYlGn: [ 'rgb(252,141,89)', 'rgb(255,255,191)', 'rgb(145,207,96)' ],
     RdBu: [ 'rgb(239,138,98)', 'rgb(247,247,247)', 'rgb(103,169,207)' ],
     ...
     },
  Qualitative:{ 
     Set2: [ 'rgb(102,194,165)', 'rgb(252,141,98)', 'rgb(141,160,203)' ],
     Accent: [ 'rgb(127,201,127)', 'rgb(190,174,212)', 'rgb(253,192,134)'],
     Set1: [ 'rgb(228,26,28)', 'rgb(55,126,184)', 'rgb(77,175,74)' ],
     ...
     },
  Sequential:{ 
     OrRd: [ 'rgb(254,232,200)', 'rgb(253,187,132)', 'rgb(227,74,51)' ],
     PuBu: [ 'rgb(236,231,242)', 'rgb(166,189,219)', 'rgb(43,140,190)' ],
     BuPu: [ 'rgb(224,236,244)', 'rgb(158,188,218)', 'rgb(136,86,167)' ],
     ... 
   } 
}
```

This is an object with the color for each type of color scheme and for each color scheme name with 3 classes.