# gulp-dojo

[![NPM version](https://badge.fury.io/js/gulp-svn2.png)](http://badge.fury.io/js/gulp-svn2)
<table>
<tr>
<td>Package</td><td>gulp-dojo</td>
</tr>
<tr>
<td>Description</td>
<td>Build Dojo inside a Gulp task</td>
</tr>
<tr>
<td>Node Version</td>
<td>>= 0.11.12</td>
</tr>
<tr>
<td>Gulp Version</td>
<td>3.x</td>
</tr>
</table>

## Install
    npm install gulp-dojo --save
    
### Usage

```javascript
  options: {
    // You can also specify options to be used in all your tasks
    dojo: 'path/to/dojo.js', // Path to dojo.js file in dojo source
    load: 'build', // Optional: Utility to bootstrap (Default: 'build')
    profile: 'app.profile.js', // Profile for build
    profiles: [], // Optional: Array of Profiles for build
    appConfigFile: '', // Optional: Config file for dojox/app
    package: '', // Optional: Location to search package.json (Default: nothing)
    packages: [], // Optional: Array of locations of package.json (Default: nothing)
    require: '', // Optional: Module to require for the build (Default: nothing)
    requires: [], // Optional: Array of modules to require for the build (Default: nothing)
    action: '', // Optional: Build action, release, help. clean has been deprecated.
    cwd: './', // Directory to execute build within
    dojoConfig: '', // Optional: Location of dojoConfig (Default: null),
    // Optional: Base Path to pass at the command line
    // Takes precedence over other basePaths
    // Default: null
    basePath: '',
    ignoreErrors: true // Options (default: false): Grunt task returns successful even if there are errors in the dojo build
  }
  gulp.task('dojobuild',function(cb){
	gudojo.dojo(options,cb);
});
```
