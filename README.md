# Testcli

This project demonstrates a workaround for [Angular CLI issue #9729](https://github.com/angular/angular-cli/issues/9729).

The relevant code is in `.vscode/launch.json`, in particular:

    "webRoot": "${workspaceFolder}",
    "sourceMapPathOverrides": {
      "webpack:/*": "${webRoot}/*"
    }

In Visual Studio Code,

- `Ctrl + Shift + B` (or Tasks > Run Build Task...)
- Set a breakpoint in `src/app/app.component.ts:9`
- Hit `F5` (or Debug > Start Debugging)
- Refresh the page and the breakpoint should be hit

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.7.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
