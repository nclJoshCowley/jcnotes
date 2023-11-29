# Angular Notes Fragment

## Angular Installation

See <https://angular.io/tutorial/first-app> for official guided tutorial.

Installed `node` via [NodeJS](https://nodejs.org/en/download) that comes
with Node package manager (`npm`).

```bash
node --version
# v18.17.1

npm --version
# 9.6.7
```

Installed Angular using

```bash
npm install -g @angular/cli

ng version
#
#      _                      _                 ____ _     ___
#     / \   _ __   __ _ _   _| | __ _ _ __     / ___| |   |_ _|
#    / △ \ | '_ \ / _` | | | | |/ _` | '__|   | |   | |    | |
#   / ___ \| | | | (_| | |_| | | (_| | |      | |___| |___ | |
#  /_/   \_\_| |_|\__, |\__,_|_|\__,_|_|       \____|_____|___|
#                 |___/
#
#
# Angular CLI: 16.2.0
# Node: 18.17.1
# Package Manager: npm 9.6.7
# OS: win32 x64
```

## TypeScript Installation

It can also be useful to install TypeScript.

```bash
npm install -g typescript

tsc --version
# Version 5.1.6
```

And then we can compile TypeScript files (`*.ts`) into JavaScript (`*.js`)
and run the JavaScript version with node.

```bash
tsc my-script.ts
# > Creates "my-script.js"

node my-script.js
# > Runs "my-script.js"
```

## New Project

We can create a new project with Angular (`ng`).

```bash
ng new project-name
```

Prompts are relatively straightforward and ask about routing, anonymous data
usage and which type of style file (`CSS`, `SCSS`, `Sass`, etc.)

Checked the app runs by using

```bash
ng serve --open
```

Note, this can also be done with `npm start` as it runs all scripts in
`package.json`.