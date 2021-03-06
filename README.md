### Jeet grid package for Meteor (especially for [Scotty](https://github.com/juliancwirko/scotty) boilerplate)

only Stylus, because it is awesome ;) (no Scss)

### Usage

You don't need to install Meteor Stylus package it is absorbed by s-jeet.
If you have it installed just uninstall it and install only s-jeet package.

You can use it without Scotty boilerplate. Just install it:

````meteor add juliancwirko:s-jeet````

and import jeet and rupture .styl files (you can also add nib):

````
@import 'nib'
@import 'jeet'
@import 'rupture'
````
nib works well with Autoprefixer.
Autoprefixer removes unused prefixes generated by nib and nib itself is sometimes helpful with its mixins and features.

See Scotty main .styl file here: [https://github.com/juliancwirko/scotty/blob/master/client/style/style.styl](https://github.com/juliancwirko/scotty/blob/master/client/style/style.styl)

### Blog post about working with Jeet in Meteor:

[Meteor.js without Bootstrap](http://julian.io/meteor-js-without-bootstrap/)

### Awesome deps!

- [Stylus](http://learnboost.github.io/stylus/) 0.49.3
- [nib](http://visionmedia.github.io/nib/) 1.0.4
- [autoprefixer-stylus](https://github.com/jenius/autoprefixer-stylus) 0.4.0
- [Jeet](https://github.com/mojotech/jeet) 6.1.2
- [Rupture](https://github.com/jenius/rupture) 0.6.1

### Autoprefixer

"Parse CSS and add vendor prefixes to rules by Can I Use" - [caniuse.com](http://caniuse.com)

Demo:
````
.test
    transform translateX(20%)
````

Which compiles to:
````
.test {
    -webkit-transform: translateX(20%);
    -ms-transform: translateX(20%);
    transform: translateX(20%);
}
````

Always actual, based on Caniuse.com!


### Changelog

- 0.2.6 Autoprefixer and Rupture versions bump
- 0.2.5 Stylus version bump
- 0.2.4 Autoprefixer version bump
- 0.2.3 Stylus and Nib versions bump
- 0.2.2 Jeet version bump
- 0.2.1 Jeet 6 on board
- 0.2.0 now with Autoprefixer
- 0.1.0 better approach with compile plugin (based on the [Meteor Stylus package](https://github.com/meteor/meteor/tree/devel/packages/stylus))
- 0.0.5 init
