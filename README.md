Generator-Fronty
=========

Simple frontend boilerplate built on yeoman, bower and grunt.

``` bash
npm install -g generator-fronty
cd myProjectFolder
yo fronty
```

### Commands:
``` bash
grunt [build] # build project
grunt server # connect server with livereload for prototyping
grunt server:dist # build and load server
grunt prebuild # fast build with no minification for debugging
grunt wPre # prebuild with watch
grunt wPre:server # prebuild with watch and server
grunt addB:name # add block with html,sass,coffee files and add it to styles/_blocks.sass
grunt removeB:name # remove block
grunt updateBlockList # updates blocks.sass
grunt static:name # add static page
```

### Prototypes navigation:
* Ctrl+SHift+X
* 3 double taps with two fingers

### Dependencies:
* Ruby:
    * Sass
    * Compass
    * Foundation (optional)
* Node.js:
    * Grunt-cli
    * Bower
    * bower

### TODO
* Change fastClick.js in foudnation to external dependency when they remove it from fw source.
* rewrite protonav
* update imagemin, still get error "building is not supported on win32", because of node-jpegtran-bin.
* make second UseminPrepare task with no minification (2.0 throws error, waiting for npm publish)
* add tests

## Release History
* 2.1.0 Compass and Ruby Sass changed to node-sass (it's really fast 5-10x)
* 2.0.0 Foundation 5 is here and set by default
* 1.2.0 .html files changed to .mustache, minor fixes in gruntfile
* 1.1.0 Static pages added, code refactoring done
* 1.0.0 Here is Fronty!