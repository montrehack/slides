# MontreHack slides

## Pre-reqs

Install [asciidoc](http://www.methods.co.nz/asciidoc/) for your platform

## Rendering documents

    $ asciidoc --attribute stylesheet=`pwd`/styles/montrehack.css \
            -o presentation.html <file>

Will render in `presentation.html`

For absolute best rendering, due to the use of a background url() call, you
should make sure you have Internet access before opening the slides (or reload
after having access).
