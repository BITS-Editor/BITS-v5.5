logolinks.jpg 220px breit, 140px hoch

header.jpg 960px breit, 140px hoch



Das Icon für externe Links wird generell in der css\bits\bits.css ab ca. Zeile 299 geregelt: 
a[href^="http://"]:before,
a[href^="https://"]:before {
 background-image: url(../../bits/images/design/extern.gif);
 background-repeat: no-repeat;
 padding-right:  15px;
}
