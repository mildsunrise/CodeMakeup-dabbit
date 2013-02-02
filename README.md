> This is a member of the [CodeMakeup](https://github.com/jmendeth/CodeMakeup) collection.
> License, other themes and common facts are listed there.

# Dabbit

**Read [How to Use](#how-to-use) below for how to launch a _demo server_,  
_use_ or _hack_ on this theme, it's super easy.**

This is the theme [Dabblet](http://dabblet.com) (the fantastic [open-source](https://github.com/LeaVerou/dabblet) design playground)  
uses. Now ported to CodeMirror, with [little modifications](#modifications).

<!-- TODO: screenshot -->

This is a **minimalist** theme. His big, but **invisible gutter** makes you focus  
on the code instead of the controls. The font size is quite large by default, but  
you can change that, and shadows & other effects will proportionally scale as well.

## License

The theme itself has been ported to CodeMirror by me, [Xavier Mendez](https://github.com/jmendeth) and is  
made available (as all other themes) under a [2-clause BSD](http://opensource.org/licenses/bsd-license), see `LICENSE`.

However, the [Gray Jean](http://subtlepatterns.com/grey-jean/) pattern that is used as background  
requires you to give credits to [Subtle Patterns](http://subtlepatterns.com). If you don't  
like that, you can use the [original noise](https://github.com/LeaVerou/dabblet/blob/8da489da6aaf4d547af58113ceaea544e104b2ce/img/noise.png), but that's less sexy!

## Modifications

It isn't a perfect imitation, because I:

 - Used [Inconsolata](http://www.google.com/webfonts/specimen/Inconsolata), an open-source beautifult monospace font
   very similar to Monaco (the propietary font only available on Macs). This is  
   because of three reasons:
   
   1. This is open-source, the font should also be.
   2. It's not a good practise to discriminate platforms, especially open-source ones.
   3. Inconsolata has better angle-brackets and `*`.
   4. Multiplatform editor (CodeMirror), multiplatform theme (Dabbletted), multiplatform font (Inconsolata).  
      Everything fits.

 - Used one of [SubtlePatterns](http://subtlepatterns.com) textures for the  
   background (Gray Jean), instead of the default noisy pattern.
 - Fixed some little bugs.

## How to use

The precompiled, ready-to-use stylesheet is on `dist/`.  
Just `<link>` to it on your page, then let CodeMirror use it:

```javascript
var editor = CodeMirror.fromTextArea(myTextArea, {theme:'dabbit'});
```

### Editing the theme

You should edit the source files at `src/`; they  
are written with the fantastic [Stylus](http://learnboost.github.com/stylus) and (NIB)(http://visionmedia.github.com/nib/).

Whenever you rename, add or remove files you may  
need to modify `theme.json` (the theme definition).  
Then to recompile the theme, just run:

```bash
./compile
```

It'll print detailed messages if something fails to compile.  
**Note:** you must have Node and NPM installed.

### Sample Server

You can also launch a webserver to try the theme:

```bash
./demo
```

It'll print the URL you have to browse.
Quirk the demo page at `manager/index.blade` and `manager/public/`.
