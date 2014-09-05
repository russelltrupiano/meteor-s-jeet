### Jeet grid package for Meteor (especially for [Scotty](https://github.com/juliancwirko/scotty) boilerplate)

only Stylus, because it is awesome ;) (no Scss)

### Usage

You can use it without Scotty boilerplate. Just install it: 

````meteor add juliancwirko:s-jeet```` 

and import jeet and rupture .styl files:

````
@import 'jeet'
@import 'rupture'
````

See Scotty main .styl file here: [https://github.com/juliancwirko/scotty/blob/master/client/style/style.styl](https://github.com/juliancwirko/scotty/blob/master/client/style/style.styl)

### Awesome deps!

- [Stylus](http://learnboost.github.io/stylus/) 0.48.1
- [nib](http://visionmedia.github.io/nib/) 1.0.3
- [autoprefixer-stylus](https://github.com/jenius/autoprefixer-stylus) 0.3.0
- [Jeet](https://github.com/mojotech/jeet) 5.3.0
- [Rupture](https://github.com/jenius/rupture) 0.4.0

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

- 0.2.0 now with Autoprefixer 
- 0.1.0 better approach with compile plugin (based on the [Meteor Stylus package](https://github.com/meteor/meteor/tree/devel/packages/stylus))
- 0.0.5 init
