# design-system-demo
--------

This project accompanies a presentation [Melanie Archer](http://twobanjos.com) prepared to introduce the concept of [design systems](https://css-tricks.com/design-systems-building-future/). It is a very small [ExpressJS](http://expressjs.com/) app offering a single page that includes some HTML form markup. Note that the form has no action, and does not submit, nor do any of the HTML links work.

Each branch of this repository shows a different state of the project as a design system is applied to it:

* 1-master
* 2-add-design-system
* 3-add-html-class
* 4-theme-design-system

To navigate between branches, use Git:
````shell
git checkout [branch name]
````


## Requirements
--------
You must have [Node.js](https://nodejs.org/en/) already installed.



## Getting started
--------
Install this project's dependencies:

````shell
npm install
````

Start the server:
````shell
npm start
````

`CTRL+C` will stop the server.

## Extras
You can compare the visual output of two different branches with [argus-eyes](https://github.com/arguseyes/argus-eyes). For instance, to check for differences between `1-master` and `4-theme-design-system`, use the following:
````shell
git checkout 1-master
argus-eyes capture 1-master

git checkout 4-theme-design-system
argus-eyes capture 4-theme-design-system

argus-eyes compare 4-theme-design-system 1-master  --verbose
````

argus-eyes will produce screenshots of each state, and report the differences on the command line.
````shell
argus-eyes compare 4-theme-design-system 1-master --verbose
[2016-04-20T20:41:13.458Z] [verbose] Found a total of 6 screenshots on the left side
[2016-04-20T20:41:13.461Z] [verbose] Found a total of 6 screenshots on the right side
[2016-04-20T20:41:13.510Z] [verbose] Image dimensions differ left and right: 1366x768/index/email-input.png
[2016-04-20T20:41:13.510Z] Difference (10.91%) above threshold (0%) found for: '1366x768/index/email-input.png'
````
