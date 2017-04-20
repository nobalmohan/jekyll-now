---
layout: post
title: Getting started with Angular CLI
tags: Angular JavaScript Technology Web
---

The Angular CLI is a command line interface tool that was released as part of Angular 2. It helps you to scaffold, develop, test, lint and deploy angular apps.

### Install Angular CLI
```
npm install -g @angular/cli
```

### Create new project
```
ng new angular-project
```

You can supply more optional params to *new* command. More [options here](https://github.com/angular/angular-cli/wiki/new#options)

### Serve your project
```
cd new-project
ng serv
```

If you want to change port, proxy, SSL certificate and all other server config. More [options here](https://github.com/angular/angular-cli/wiki/serve#options)

### Test your app with karma

```
ng test
```
Test will automatically run after build. Test command is in live-reload mode. If you want to execute it only once. Add flag *--watch=false*. More [options here](https://github.com/angular/angular-cli/wiki/test#options)

### Lint your app

You can list your entire application using *tslint* with the command. More [options here](https://github.com/angular/angular-cli/wiki/lint)

```
ng lint
```
### Building your app

Build command compiles your application into a output directory.

```
ng build
```
You can customized both a build target and an environment by passing --target and --environment flags respectively. More [options here](https://github.com/angular/angular-cli/wiki/build)

### angular-cli.json

Any default values can be overridden in *angular-cli.json* at the root level generated during *ng new* command.


## More wiki about customizing Angular CLI [here](https://github.com/angular/angular-cli/wiki/stories)
