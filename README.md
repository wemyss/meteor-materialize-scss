# INSTALL
```
$ meteor add fourseven:scss
$ meteor add swemyss:materialize-scss
```

# SCSS
Add the following lines to your last-loaded scss file (E.G. main.scss):
```
// If you want to override materialize sass variables you can uncomment the following:
// @import "{swemyss:materialize-scss}/sass/components/_color.scss";
// $primary-color: color("blue", "lighten-2");

// import main scss file
@import "{swemyss:materialize-scss}/sass/materialize.scss";
```

# ICONS
Icons that are a part of materialize are not included in this project as they are limited in their use (as opposed to FontAwesome).

# JAVASCRIPT
Javascript is automatically imported from this package.

# CHANGE LOG

- 2016-01-28 update to materializecss [0.97.5](https://github.com/Dogfalo/materialize/tree/v0.97.5#changelog)
- 2015-11-22 update to materializecss [0.97.3](https://github.com/Dogfalo/materialize/tree/v0.97.3#changelog)

- 2015-10-01 update package for METEOR@1.2 (*Breaking*)
  - fourseven:scss is updated to 3.3.3_1
  - scss.json is not used anymore.
  - index.scss is not autoupdated anymore, you need to manullay update index.scss.

# FOR MAINTAINERS

- HOW TO UPDATE TO NEW VERSIONS OF MATERIALIZECSS
```
git checkout master
git pull https://github.com/Dogfalo/materialize.git master --tags
git checkout <previous-mms-version-on-github>
git checkout -b <next-mms-version>
git rebase <latest-stable-materializecss-version>
// check if we need to add new files to package.js
// change meteor package version
// test
meteor publish
```
