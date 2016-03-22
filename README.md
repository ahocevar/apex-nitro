# APEX Front-End Boost
[![Build Status](https://travis-ci.org/OraOpenSource/apex-frontend-boost.svg?branch=master)](https://travis-ci.org/OraOpenSource/apex-frontend-boost)
[![Dependency Status](https://david-dm.org/OraOpenSource/apex-frontend-boost.svg)](https://david-dm.org/OraOpenSource/apex-frontend-boost)

This productivity tool helps you work with web files (`js`, `css`, `images`, etc.) more efficiently within an APEX application.

APEX Front-End Boost is first and foremost a personal local web server that hosts and distributes your files to your APEX application.

TODO Martin: include animated gif (#19) of this project in action.

**What APEX Front-End Boost does:**
- Minifies `css` and `js`.
- Generates  `js` and `css` sourcemaps.
- Adds `css` vendor prefixes.
- Concatenates `css` and `js`. *(optional)*
- Parses `scss` and `less` to `css`. *(optional)*
- Generates APEX Theme Roller configuration. *(optional)*
- Transforms `css` to RTL format. *(optional)*

**What APEX Front-End Boost allows you:**
- Cutting down on front-end development time.
- Enhance your application performance due to smaller file sizes.
- Keep coding in your favorite code editor, without having to constantly upload anything to APEX or a web server.
- Stop manual refresh of your browser to get `js` and `css` modification.
- Stop worrying about affecting other developers. Any development done within APEX Front-End Boost affects you and only you.
- Be notified of `js` and `css` errors as you save.

It makes responsive development easier by synchronizing multiple devices together. Your desktop, tablet and mobile device will imitate each others actions (scrolling, clicking, typing) as long as you've got APEX Front-End Boost running.

It eliminates the need for refreshing the browser. As soon as you save your code in the text editor, you get automatic code injection / reloading in the browser.

All of it is very much instantaneous.

APEX Front-End Boost does make coding faster, richer and prettier, in addition to providing a better performance to the browser.

## Project Sponsors
Thanks to [Insum Solutions](http://insum.ca/) for sponsoring this project.

## Install
```bash
git clone https://github.com/OraOpenSource/apex-frontend-boost.git
cd apex-frontend-boost
npm install
```

**Installing on Windows?** [See documentation](/docs/windows.md).

## APEX Front-End Boost Configuration
You need to configure APEX Front-End Boost for your project(s). [See documentation](/docs/config.json.md).

## APEX Application Setup
There are two options to setup your application:
- **Option 1) Standard**
    - 1 Build Option
    - 1 Application Process
- **Option 2) Custom Application Item**
    - 1 Build Option
    - 1 Application Item
    - 2 Application Processes

Review the [APEX Setup](/docs/apex-setup.md) docs to choose the most appropriate option for your project.

## Run
`npm start -- --project=yourProjectName`

**Running on Windows?**
- Execute `apex-frontend-boost` shortcut
- Enter project name

**[Running a real OS](http://stackoverflow.com/research/developer-survey-2016#technology-desktop-operating-system)? Linux/OSx Shortcut:**
- `./apex-frontend-boost.sh`
- Enter project name

## Usage
From the `src` folder you can create, edit or delete any files in:
```
|-/src/
	|-scss
	|-less
    |-css
    |-img
    |-js
    |-lib
```

APEX Front-End Boost will automatically compile your files to this folder structure:
```
|-/dist/
    |-css
    |-img
    |-js
    |-lib
```

#### Using with multiple devices
[See documentation](/docs/multiple-devices.md).

#### Self-Signed SSL Browser Warning
[See documentation](/docs/ssl-warning.md).

## Features
- [Browsersync](http://www.browsersync.io/)
- [Sass](http://sass-lang.com/)
- [Less](http://lesscss.org/)
- [Autoprefixer](https://github.com/postcss/autoprefixer)
- [JSHint](http://jshint.com/)
- [UglifyJS](https://github.com/terinjokes/gulp-uglify)
- [Sourcemaps](https://www.npmjs.com/package/gulp-sourcemaps)
- [RTLCSS](https://github.com/MohammadYounes/rtlcss)
- More...

[See features examples](/docs/examples.md).

## Changelog
[See changelog](changelog.md).

## Project Team
- [Vincent Morneau](https://twitter.com/vincentmorneau)
- [Martin Giffy D'Souza](https://github.com/martindsouza)
