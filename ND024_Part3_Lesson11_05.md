# Lesson 11.5 Install Gulp

### Installing Gulp and Course Code
Note: if you have not installed NodeJS or NPM you will need to install these first before installing Gulp. You can download and install NodeJS and NPM by going to Nodes official site and downloading the latest version of NodeJS.

1. Take a few moments and install [Gulp](https://github.com/gulpjs/gulp/blob/master/docs/getting-started.md). The instructions are listed in the link.
2. Grab the course code from [Github](https://github.com/udacity/ud892).

1. Install Gulp

Getting Started
If you've previously installed gulp globally, run npm rm --global gulp before following these instructions. For more information, read this Sip.

Check for Node and npm
Make sure that you've installed Node and npm before attempting to install gulp.

node --version
npm --version
Install the gulp command
npm install --global gulp-cli
Create a package.json in your project directory
If you don't have a package.json, create one. If you need help, run an npm init which will walk you through giving it a name, version, description, etc.

Install gulp in your devDependencies
Run this command in your project directory:

npm install --save-dev gulp@next
Create a gulpfile
In your project directory, create a file named gulpfile.js in your project root with these contents:

var gulp = require('gulp');

gulp.task('default', defaultTask);

function defaultTask(done) {
  // place code for your default task here
  done();
}
Test it out
Run the gulp command in your project directory:

gulp
To run multiple tasks, you can use gulp <task> <othertask>.

Result
Voila! The default task will run and do nothing.

Using gulpfile ~/my-project/gulpfile.js
[11:15:51] Starting 'default'...
[11:15:51] Finished 'default' after 103 μs
.src, .watch, .dest, .parallel, .series, CLI args - How do I use these things?
For API specific documentation, you can check out the documentation for that.

Where do I go now?
API Documentation - The programming interface, defined
Recipes - Specific examples from the community
In Depth Help - A tutorial from the guy who wrote the book
Plugins - Building blocks for your gulp file






- - -
Next up: [Hello Gulp](ND024_Part3_Lesson11_06.md) or return to [Table Of Contents](./ND024_TableOfContents.md)
