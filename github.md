# SECWall Frontend app.

## Featuring
 - react
 - react-router with Home About and 404
 - gulp as a build system
 - npm as module manager

## Prequisities
Web part of the poroject required  <code>**NodeJS v4.0.0**</code>
Instalation Guide: http://mycodesmells.com/post/node-version-management/

You need to run
`npm install`

## Gulp tasks
All task are in the _gulp/tasks/ folder:


[//]: # (Two trailing white-spaces breaks a line)
`./gulp.sh` - default: will compile all and watch file changes  
`./gulp.sh build` - will build app  
`./gulp.sh clean` - will remove build artifacts  
`./gulp.sh test` - check unit tests  
`./gulp.sh test -t test-path` - check unit tests from one file  
`./gulp.sh tdd` - check unit tests and watch changes in the file  
`./gulp.sh tdd -t test-path` - check unit tests and watch changes from one file  

## Production
`./gulp.sh build --type production` To build uglyfied version.


## Styles folder structure

```
...
|
└── css/
    |
    ├── components/
    |   |   _buttons.less
    |   |   _fonts.less
    |   |   _modal.less
    |   └── ...
    |
    ├── mixins/
    |   |   _responsive.less
    |   └── ...
    |
    ├── modules/
    |   |   _connection-watch.less
    |   |   _login.less
    |   |   _tour-guide.less
    |   └── ...
    |
    ├── themes/
    |   ├── widgets/
    |   |    _chart-widget.less
    |   |    _killchain-widget.less
    |   |    _value-widget.less
    |   |    _widget.less
    |   |
    |   ├──  _main.less
    |   ├──  _navigation.less
    |   ├──  _share.less
    |   ├──  _sidebar.less
    |   └──  _theme-vital-dark.less
    |
    ├── sections/
    |   |   navigation.less
    |   |   login.less
    |   |   tour-guide.less
    |   └── ...
    |
    |   _helpers.less
    |   _layout.less
    |   _layout-responsive.less
    |   _variables.less
    └── styles.less
```
