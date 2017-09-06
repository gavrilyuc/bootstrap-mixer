# Bootstrap Mixer

This is addition to bootstrap, includes mixing classes and easy way to style blocks.<br />
It helps to improve using repetitive styles.

## Instalation

> npm install bootstrap-classmixer
or
> bower install bootstrap-classmixer

## Compiling sources

Installing [Koala](http://koala-app.com/) ([github project](https://github.com/oklai/koala/)), or
Download sass compiler:
* **Windows**
    Before you start using Sass you will need to install Ruby. The fastest way to get Ruby on your Windows computer is to use [Ruby Installer](https://rubyinstaller.org/). It's a single-click installer that will get everything set up for you super fast.
    The installer will also install a Ruby command line powershell application that will let you use the Ruby libraries.

    Then open prompt console(`Win+R > cmd.exe`) and install ssas.
    > gem install sass
* **Linux**
    If you're using a distribution of Linux, you'll need to install Ruby first. You can install Ruby through the apt package manager, rbenv, or rvm.
    Then 
> sudo gem install sass

After that compile sources: [see sass documentation](http://sass-lang.com/)

> sass --watch bootstrap-classmixer.scss:bootstrap-classmixer.css --style compressed

## Using and information

`padding-left-50` -> added padding-left 50 **pixels**;<br />
`padding-left-50pr` -> added padding-left 50 **procent**;<br />
`padding-left-50vw` -> added padding-left 50 **vw**;<br />

```html
<div class="padding-top-50 background-color-black">
  Example text
</div>
```
You may use multi screens classes: `lg-*`, `md-*`, `sm-*`, `xs-*`
```html
<div class="lg-padding-top-150 md-padding-top-100 sm-padding-top-50 xs-padding-top-0">
  Example text
</div>
```
Using default web colors:
```html
<div class="lg-color-red md-color-silver sm-color-pink xs-color-black">
  Example text
</div>
```
Using font size:
```html
<div class="lg-font-26pt md-font-23pt sm-font-18 xs-font-16">
  Example text
</div>
```
## Full example
```html
<div class="row">
    <div class="col-xs-12">
        <div class="lg-padding-top-30 lg-padding-bottom-30 xs-padding-0">
            Example Padding top (large window: top/bottom 30px, other 0px)
        </div>
    </div>
    <div class="col-xs-12">
        <div class="lg-color-black md-color-gay sm-color-silver xs-color-white sm-backgroun-white xs-background-black">
            Example color styling
        </div>
    </div>
    <div class="lg-font-28pt md-font-26pt sm-font-22pt xs-font-18pt">
        Font size styling
    </div>
</div>
````
