# AngularScssWindowsAotIssue

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.2.2.

## Issue description

Changes in partial scss (starting with `_`) files are not respected during `ng serve --aot` on Windows. Everything works fine on Ubuntu and macOS. Everything works fine when `--aot` is not passed.

## Steps to reproduce
1. Clone this repo: `git clone https://github.com/rosen-vladimirov/angular-scss-windows-aot-issue.git`
2. In the project run `ng serve --aot`
3. Apply a change in `src/app/_colored_classes.scss` - the change will not be respected