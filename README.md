# Ng6ClrApp

Setup the Angular 6 project with VMware clarity
================================================

Step 1) npm install –g @angular/cli
Step 2) ng new project-name –style=scss --routing
Step 3) cd project-name
Step 4) npm install @clr/icons @webcomponents/custom-elements @clr/ui @clr/angular rxjs-compat –save
Step 5) Include “import { ClarityModule } from '@clr/angular';” and add in imports: [….,ClarityModule, …] in “app.module.ts” file.
Step 6) Modify “angular.json” file with the below code.

         "styles": [
              "src/styles.scss",
              "./node_modules/@clr/icons/clr-icons.min.css",
              "./node_modules/@clr/ui/clr-ui.min.css"
            ],
            "scripts": [
              "./node_modules/@webcomponents/custom-elements/custom-elements.min.js",
              "./node_modules/@clr/icons/clr-icons.min.js"
            ]

Step 7) To test add some clarity ui components ( take from https://vmware.github.io/clarity/documentation/v0.11/header ) in “app.component.html” file.
Step 8) ng serve –o