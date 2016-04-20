# design-system-demo

This project accompanies a presentation [Melanie Archer] prepared to introduce the concept of [design systems]. It is a very small [ExpressJS|http://expressjs.com/] app offering a single page that includes some HTML form markup. Note that the form has no action, and does not submit, nor do any of the HTML links work.

Each branch of this repository shows a different state of the project as a design system is applied to it:

* 1-master
* 2-add-design-system
* 3-add-html-class
* 4-theme-design-system

To navigate between branches, use Git:
````shell
git checkout [branch name]
````

## To install this project

Requirements
--------
You must have [Node.js|https://nodejs.org/en/] already installed.

````shell
cd design-system-demo
````

````shell
npm install
````

## Extras
You can compare the visual output of two different branches with [argus-eyes|https://github.com/arguseyes/argus-eyes]. For instance, to check for differences between `1-master` and `4-theme-design-system`, use the following:
````shell
git checkout 1-master
argus-eyes capture 1-master

git checkout 4-theme-design-system
argus-eyes capture 4-theme-design-system

argus-eyes compare 4-theme-design-system 1-master  --verbose
````

argus-eyes will produce screenshots of each state, and report on the differences on the command line.
