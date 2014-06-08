# grunt-vs-android

> Updates the manifest file with the new version name, supports both night and semver equivalent. used for CI Process

## Getting Started
This plugin requires Grunt `~0.4.4`
Also ensure [xmlstarlet](http://xmlstar.sourceforge.net/) is installed and available in the path
If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-vs-droid --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-vc-droid');
```

## The "droid" task

### Overview
In your project's Gruntfile, add a section named `droid` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  droid: {
    options: {
      mode: 'nightly' // the other option is to use semver which will update the version using semver
    },
  },
});
```
### Usage Examples
## Using the nightly mode

```bash
[rp@sodium grunt-vc-android (master ✗)]$ grunt droid:AndroidManifest.xml:build1234
Running "droid:AndroidManifest.xml:build1234" (droid) task
Current version: 4.0.1-0
The new version is 4.0.1-0+build1234
The version is now updated to 4.0.1-0+build1234

```
## Using the semver mode
```
[rp@sodium grunt-vc-android (master ✗)]$ grunt droid:AndroidManifest.xml:prepatch
Running "droid:AndroidManifest.xml:prepatch" (droid) task
Current version: 4.0.0
The new version is 4.0.1-0
The version is now updated to 4.0.1-0
```

Check out documentation for semver  to see the options that can be passed

## Contributing

## Release History
