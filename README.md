# Sistema
* Criar o sistema com o comando ng new sistema

* Na estrutura do projeto no vscode ou outra idei que utilize para trabalho, adicione as seguintes dependencia no projejeto:

* npm install --save-dev electron && npm i electron-builder

* O package.json ficará nesta forma:

{
  "name": "MQS-sistema_Demo",
  "main": "main.js",
  "version": "0.0.0",
  "scripts": {
    "ng": "ng",
    "start": "ng serve",
    "build": "ng build",
    "watch": "ng build --watch --configuration development",
    "test": "ng test",
    "serve:ssr:sistema": "node dist/sistema/server/server.mjs",
    "electron": "ng build --base-href ./ && electron .",
    "dist": "ng build --base-href ./ && electron-builder"
  },
  "private": true,
  "dependencies": {
    "@angular/animations": "^19.1.0",
    "@angular/common": "^19.1.0",
    "@angular/compiler": "^19.1.0",
    "@angular/core": "^19.1.0",
    "@angular/forms": "^19.1.0",
    "@angular/platform-browser": "^19.1.0",
    "@angular/platform-browser-dynamic": "^19.1.0",
    "@angular/platform-server": "^19.1.0",
    "@angular/router": "^19.1.0",
    "@angular/ssr": "^19.1.4",
    "express": "^4.18.2",
    "rxjs": "~7.8.0",
    "tslib": "^2.3.0",
    "zone.js": "~0.15.0"
  },
  "devDependencies": {
    "@angular-devkit/build-angular": "^19.1.4",
    "@angular/cli": "^19.1.4",
    "@angular/compiler-cli": "^19.1.0",
    "@types/express": "^4.17.17",
    "@types/jasmine": "~5.1.0",
    "@types/node": "^18.18.0",
    "electron": "^34.0.2",
    "electron-builder": "^25.1.8",
    "eletron": "^0.0.1-security",
    "jasmine-core": "~5.5.0",
    "karma": "~6.4.0",
    "karma-chrome-launcher": "~3.2.0",
    "karma-coverage": "~2.2.0",
    "karma-jasmine": "~5.1.0",
    "karma-jasmine-html-reporter": "~2.1.0",
    "typescript": "~5.7.2"
  },
  "build": {
    "appId": "software.mqs",
    "productName": "MQS-Sistemas",
    "mac": {
      "category": "public.app-category.developer-tools"
    },
    "files": ["**/*", "dist/sistema/browser/**"]
  }
}

