# quick-setup
Quick Setup File


## Dependancies

* Ruby (preinstalled on macOS)

* Sass, requires Ruby

---

## Installing Ruby

**Windows / macOS**

* Click on this [link](https://rubyinstaller.org/), download the package, follow the instructions.

---

## Installing Sass

**Windows / macOS**

* In terminal (mac) or cmd (windows) enter `sudo gem install sass`, you will need to remove the `sudo` from windows.

* Enter `sass -v` to verify the install completed successfully

* If none of this works, consult the [sass install guide](http://sass-lang.com/install)

--- 

## Running Sass on Your Project

Simply open a terminal / cmd, and navigate to your project directory and type

`sass --watch --no-cache --sourcemap=none scss:css --style=compressed`

---

## Breakdown of the Sass Parameters

`--watch`

Tells sass to watch for changes to scss files then compile when one is detected

---

`--no-cache`

This removes the default caching that sass does. For our purposes and the speed at which it compiles. Even in our larger projects this is not an issue, so we remove it as it would be excess that that is hidden and would get committed with our work.

---

`--sourcemap=none`

A source map is useful for mapping a css file to it's corresponding sass file. Chrome makes use of this in dev tools when one it spotted. They will create extra files for every outputted css file. Typically not my preference and I don't like adding additional fluff to our commits. Here is a good resource on [how to use source maps in chrome](https://robots.thoughtbot.com/sass-source-maps-chrome-magic)

---

`scss:css`

Simply the source directory, scss, and then the output directory css.

--- 

`--style=compressed`

This minifys the css file to be smaller and quicker to read, additionally it'll strip out all the comments as well.

To see the different output styles, please refer to [here](https://web-design-weekly.com/2014/06/15/different-sass-output-styles/)
