# StewMac fret template generator

This is a work-in-progress script that generates fret-slotting templates
for the [Stewart-MacDonald Fret Slotting Table Saw Blade][1]. The script
generates the template as an SVG file, then you can make an acrylic
template on your laser cutter.

I don't have the StewMac miter box, so I don't know if it works with
that or not. I imagine that you could modify the script to make it
work, though.

##  Instructions

It's super easy.

### If you like `pipenv`:

```bash
pipenv install
pipenv run ./fretcalc 24.75 22 # make a 24.75" scale template with 22 fret slots
```

### If you don't like `pipenv`:

```bash
pip install svgwrite
./fretcalc 24.75 22 # make a 24.75" scale template with 22 fret slots
```

## Questions

### Have you tested this?

Nope.

### Can I use this to make the nut slot on a Fender-style fingerboard?

Not yet, but I'm going to add an option for that really soon.

### Why are you using inches instead of millimeters?

The only fretted instrument that I know of with a neck scale measured
in millimeters is the classical guitar, with a 650mm scale. Banjos,
ukuleles, electric guitars, and steel-string acoustic guitars usually
have neck scales specified in inches. I'll support metric units
when I'm confident that everything else is working right.

## Future Improvements

* Actually testing it by making a real, physical fretboard.
* Support for Fender-style nut slots
* Support for metric units (e.g. 650mm scale classical guitars)

[1]: https://www.stewmac.com/luthier-tools-and-supplies/types-of-tools/saws/fret-slotting-table-saw-blade/
