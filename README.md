![Kongkow IT Pekanbaru Logo](assets/page-logo.png)

# assets.kongkowitpku.xyz

Website with Kongkow IT Pekanbaru brand assets

## Update assets

If you change the SVG assets, you need to re-render the assets in the PNG and PDF folders to keep them in sync.

_Note: The commands below work on Fedora, but on Debian-based systems you have to replace `rename` with `rename.ul`._

Navigate to the SVG folder:

```
cd assets/svg
```

Render the PNGs:

```
for f in *.svg ; do rsvg-convert -f png -x 2 -y 2  $f -o $f.png ; done && rename .svg.png .png * && mv *.png ../png
```

Render the PDFs:

```
for f in *.svg ; do rsvg-convert -f pdf -x 2 -y 2  $f -o $f.pdf ; done && rename .svg.pdf .pdf * && mv *.pdf ../pdf
```

## License

<a href="https://creativecommons.org/licenses/by-sa/4.0/">
  <img align="right" height="96" alt="CC BY-SA 4.0" src="https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by-sa.svg" />
</a>

Kongkow IT Pekanbaru logo are licensed under the **CC BY-SA 4.0**.

The full text of the license can be accessed via [this link](https://creativecommons.org/licenses/by-sa/4.0/) and is also included in the [license](LICENSE) file of this software package.
