This is a template for kickstarting a CodeMakeup quickly. Steps:

 1. Learn how to edit/write the theme on "How to Use" below.
 2. Rename `src/MYTHEME.styl` and edit `theme.json` and this README accordingly.
 3. Don't forget to `./compile` the theme when it's finished!
 4. Remove this text.



> This is a member of the [CodeMakeup](https://github.com/jmendeth/CodeMakeup) collection.
> License, other themes and common facts are listed there.

# My Theme

**Read [How to Use](#how-to-use) below for how to launch a _demo server_,  
_use_ or _hack_ on this theme, it's super easy.**

TODO: Explain this theme (origin, properties, where to use it)...

TODO: screenshot here

This is a **minimalist** theme. His big, but **invisible gutter** makes you focus  
on the code instead of the controls. The font size is quite large by default,  
but you can change that, and shadows & other effects will proportionally scale.  

## How to use

The precompiled, ready-to-use stylesheet is on `dist/`.  
Just `<link>` to it on your page, then let CodeMirror use it:

```javascript
var editor = CodeMirror.fromTextArea(myTextArea, {theme:'MYTHEME'}); //TODO: adjust this
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
