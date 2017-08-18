# grunt-require-whitelist

> Validate your NinaScript package to ensure required modules are on the Engineering whitelist

## Getting Started
This plugin requires Grunt.

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install git://github.com/VirtuOz/grunt-require-whitelist --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-require-whitelist');
```

## The "require_whitelist" task

### Overview
In your project's Gruntfile, add a section named `require_whitelist` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  require_whitelist: {
    options: {
      // Task-specific options go here.
    },
    src: [ 
        //add files to be validated 
    ]
  },
})
```

### Usage Examples

#### Default Options
In this example, we validate the require statements in all .js files contained within the 'lib' directory
```js
grunt.initConfig({
  require_whitelist: {
    options: {},
    src: ['app.js','lib/**/*.js']
  },
})
```

## The “dependencyCheck” task
See the `grunt-dependency-check` [docs](https://github.com/sindresorhus/grunt-dependency-check).

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
_(Nothing yet)_

## License
Copyright (c) 2015 Matt Casella. Licensed under the MIT license.
