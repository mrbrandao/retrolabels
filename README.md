# Retro Labels

A Place To Store Labels, for floppies, minidiscs, cd-roms and others...

Turns out that sometimes we want to print or labels back to our own floppy
disks, MiniDiscs, CD-ROMs and others.  
This repository aims to be a central resource for storing and saving all labels,
and make it accessible to restore our nostalgia of printing and recreating it back
at any time.

- [Why Does this Exists?](README.md#why)
- [Contributing](README.md#contributing)
  - [Files Format](README.md#files-format)
  - [Artwork and Design Creating Tools](README.md#recommended-tools)
  - [The Retrolabels Structure](README.md#the-main-structure)
  - [Creating a new Project](README.md#creating-a-new-project)
- [Frequently Asked Questions](README.md#faq)

### Why

Sometime ago I've bought some Verbatim 3.5" floppy, and because those were old,
I was not able to use the original labels, since the glue was old and
does not work anymore. So I've decided to print back in a new sticker paper, in
order to have it as brand-new again. However! I haven't found any place were
to download the original labels. I didn't want a fake label, I want the
original, with the same brand, lines and colors, so I can write again my labels
manually as we do when we have a brand new floppies.

Since I haven't found those labels, I start to collect all diskette brands I
found and started to scan the labels, creating all the measurements to print,
and also writing back to me the instructions, so I can remember next time I have
to do it again.
I also have to save this work somewhere. So the retrolabels repository is born!

If you are like me, which still uses floppies in your retro PCs or are part of
retrocommunities and still want to revive your floppies or MiniDiscs with your
labels. This is a safe place were we can share those with every body.

Join me on, expanding this library of retrolabels.

This repository also accepts original handycraft labels, that you create to
your self and any artwork for reproducing your labels.  
For examples. lets say you're creating some nice MiniDisc label for the band
`Foo`, and you created some nice artwork. This is the place you can store and
share your original creations.

## Contributing

Feel free to contribute with this project, please send all your artwork
versions.

This repository expects artworks for re-creating floppies, Mini-Discs, CD-ROM's and
other labels.

To contribute with a new label, start with:

1. Fork this project
2. Create your awesome new artworks
3. [Create a new project to your labels](README.md#creating-a-new-project)
4. Submit a Pull Request with your project or changes

### Files Format

Since the idea here is to keep all artwork open the only rule to contribute is
to provide the artworks saved with a open standard format. For example `.SVG`
files are very welcome.

With that the rule is, to always send back the artwork in a vectorial format
compatible with [inkscape](https://inkscape.org/) using `.svg` extension, or
[GIMP](https://gimp.org) using the `.xcf` extension. The artwork must be saved
in a `art` directory inside your labels project. [Read more on how to organize
your project here.](README.md#creating-a-new-project)

That means if you are using closed source proprietary tools such as:
"Photoshop, or any other Adobe Suite, or even CorelDraw" please make sure to
export the file to an open extension, so every one can contribute back with your
artwork.

### Recommended Tools

This project does not mandate at all which tool you should or should not use.
Use whatever tool you have handy and have experience with. However for those who
does not have any, it's recommended to explore [GIMP](https://gimp.org) in favor of Adobe
Photoshop, and [Inkscape](https://inkscape.org) in favor of CorelDraw.

If you use closed tools such as Adobe Suite or CorelDraw, please make sure to
find a way to send the artwork files in a format that others who don't have access
for such tools can also contribute back.

For example:

One developing the artwork `foo.cdr` in CorelDraw can save the
`cdr` file in the `art` directory, but also the `foo.svg` file.

### Labels Structure

In order to have all labels organized this repository expects the files to
follow the same structure, which is the following:

#### The Main Structure

```bash
.
|- floppy
|- minidisc
|- cdrom
|- dvd
```

The main structure of this repository, is organized by the midia type. If you
are submitting floppies, start your structure inside the [floppy](floppy)
directory, in other hand if you're submitting MiniDiscs use the [minidisc](minidisc) directory instead.

#### Creating a new Project

When you create a new project, use the following structure:

```bash
./project-name
|- art
|- fdd312
|- fdd514
|- fonts
|- original
|- README.md
```

Where the those directories corresponds to:

- `project-name` - This is the directory name of your labels project.
  Example:  
   If you're creating labels for the Verbatim 3½-inch, your project can be
  named `verbatim`. Create it inside the main [floppy](floppy) directory.
  e.g:

  ```bash
  ./floppy/verbatim
  |- fdd312
  |- art
  ```

- `art` - This directory must be created inside your project directory, and it
  must have all the artwork you're creating. For example, `svg` and `xcf` files
  would be stored in this directory.

- `fdd312` - If the floppy diskette is a 3½-inch, the labels in final image format will
  be stored here. For example the `verbatim-label.png` file is the finished
  label file artwork ready to be printed.

- `fdd514` - This is to store the final image format ready to be printed, but
  for 5¼-inch floppies.

- `fonts` - Here you can store all fonts used in your artwork. This will
  simplify others to contribute with your project by using the properly fonts.

- `original` - All scanned and original copies of your labels, must be stored
  here. Example: The original scan copy of the Verbatim labels.

- `README.md` - The documentation of your project. Make sure to properly
  document your project, allowing other to understand how to use it. Include
  here, measurements and printing instructions on how to properly use your
  labels. Use the [`diskclub` README](floppy/diskclub/README.md) as template
  for it. Copy and adjust it to your project.

## FAQ

- Q: How can I contribute with labels?  
  A: Please jump into the [Contributing](README.md#contributing) session to know more.

- Q: Can I save the scan copies of my floppy labels?  
  A: Yes! Please do so! Scan your floppy disks and follow the [Contributing](README.md#contributing) guides, to upload your scans.

- Q: How can I print my label?  
  A: Download the label you want and follow the README in the label instructions
  to know how to recreate the size, and use the proper paper.

- Q: Can I submit only brand labels or can I submit my original labels?  
  A: Yes Please, send your original artwork, this repository is to store labels
  in general, not only brand labels, but also your manufactured original
  creations.
