# Atom Configuration


## About

This is package to configuration **atom editor**. Contains all settings, plugins and themes to work with web application.

## Instalation in Windows

Open command line as **administrator** and type:
```sh
git config --global --add core.longpaths true
```
This instruction remove long path issue on microsoft window platform.

Then type:

```sh
cd %userprofile%
git clone https://github.com/dariuszpaluch/atom-configuration
rmdir .atom
mkdir .atom
mklink /D %userprofile%\.atom\packages %userprofile%\atom-configuration\.atom\packages
mklink %userprofile%\.atom\init.coffee %userprofile%\atom-configuration\.atom\init.coffee
mklink %userprofile%\.atom\styles.less %userprofile%\atom-configuration\.atom\styles.less
mklink %userprofile%\.atom\config.cson %userprofile%\atom-configuration\.atom\config.cson
mklink %userprofile%\.atom\keymap.cson %userprofile%\atom-configuration\.atom\keymap.cson
mklink %userprofile%\.atom\snippets.cson %userprofile%\atom-configuration\.atom\snippets.cson
```

To use **sass-lint** and **eslint** in Atom, you need to install eslint and sass-lint globally by npm.
Open command line in repository folder and type:
```sh
npm run install-plugins
```
