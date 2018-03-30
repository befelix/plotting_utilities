# utilities
Some plotting utilities

### Useful latex commands

bounding box around images:
```
\usepackage[export]{adjustbox}
\includegraphics[scale=1, frame]{.....}
```

measure text/image size
```
\usepackage{printlen}
\uselengthunit{cm}
\newlength\imageheight
\newlength\imagewidth

% ...measure text width
textwidth: \printlength{\textwidth}
columnwidth: \printlength{\columnwidth}

% ...measure image size
\settoheight\imageheight{\includegraphics{img/test.eps}}
\settowidth\imagewidth{\includegraphics{img/test.eps}}

image height: \the\imageheight\ (\printlength{\imageheight}) \\
image width:  \the\imagewidth\ (\printlength{\imagewidth})
```
