# v.1.0.0
<h4>What's New?</h4>
<ul>
    <li>First Release S4 Supper Apps</li>
</ul>
# Vuexy - Angular Admin Template

This project was generated with [Angular CLI](https://github.com/angular/angular-cli).

## Adding new app inside projects
1. `git pull [hostRepo]`
2. Create a new repo for new app
3. Run `git submodule add -b [branchName] http://192.168.223.213/jefri/[appName] projects/[appName]`
4. Push changes

## Cloning certain apps (no modification inside projects/)
1. `git pull [hostRepo]`
2. `git submodule update --init` (get latest commits of all apps inside projects/)
   OR
   `git submodule update --init projects/[appName]` (get latest commits of specific apps)

3. To get newest commit of apps in existing hostRepo,
   `git submodule update --remote` (will update newest commit of all apps)
   OR
   `git submodule update --remote projects/[appName]` (update latest commits specific apps)

   
## Modifying existing app inside projects/
1. `git pull [hostRepo]`
2. `git submodule update --init projects/[appName]`
3. cd projects/[appName]
4. git checkout to tracking branch of [appName] (git checkout -b `project-[appName]`)
5. `git pull` && modify projects/[appName]
6. `git add` && `git push projects/[appName]` to its tracking branch
7. cd back to parent
8. `git add` && `git push`

## Adding webpack module-federation to apps inside projects/
1. Follow tutorial to add app inside projects
2. `ng add @angular-architects/module-federation --project [appName] --port [portNumber]` (`[appName]` is application name under `projects/` folder)

## NOTES
Setelah menambah menu di dalam menu.ts, update webpack.config.js dan juga app-routing.module.ts masing-masing apps


## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
