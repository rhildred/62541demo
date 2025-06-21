# 62541demo
using https://github.com/open62541/open62541 as submodule to make an example

```bash
git submodule update --init --recursive
mkdir build
cd build
cmake ../open62541
make

```

to build examples from https://www.open62541.org/doc/master/tutorials.html.

```
sudo make install
cd ../tutorial
gcc -std=c99 -o server tutorial_server_firststeps.c -lopen62541
```

There are lots more examples in `../open62541/examples`.

Now to figure out what all of this means. I also want to do otel with this. I think that I need https://github.com/dorsal-lab/opentelemetry-c.

I also have nginx unit installed. To run unit in the foreground:

```
sudo unitd --no-daemon --control "0.0.0.0:8080"
curl -X PUT --data-binary @nginx-unit-config.json http://localhost:8080/config
```

# AngularCustomElement

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 20.0.0. It is based on [the article](https://medium.com/@cory.lewis1997/angular-17-component-library-wired-for-web-components-3dccb87a6f87).

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
