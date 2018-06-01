# This is a work in progress document outlines Nate Framework as it is being designed. Anything can change at any time.

# What is Nate?

Nate is a native app framework for iOS and Android that provides styling designed for iOS and Android made with [Vue](https://vuejs.org/) components. It is planned to be easy to use and instead of Cordova use the upcoming [Capacitor Framework](https://capacitor.ionicframework.com/). Programming will be done in either [Typescript](https://github.com/Microsoft/TypeScript) or [ES6](https://babeljs.io/) (not decided yet) with [Vue](https://vuejs.org/). [Webpack](https://webpack.js.org/) will do all of the convesion and compessing fun stuff.

# File System (todo)

```
/node-modules
/build
/src
    /components
    /pages
    index.html
    index.js
package.json
```

# Nate-cli

```
> nate
```

Creates new project if there are none or verifies project (see nate verify).

```
> nate info
```

Prints info about nate.

```
> nate generate [name]
```

or

```
> nate new project [name]
```

Generates a new project (see file system).

```
> nate help
```

or

```
> nate -h
```

or
```
> nate [command(s)] -h
```

Get commands or subcommands.

```
> nate new compnent [name]
```

Create new vue component.

```
> nate new page
```

Creates new page.

```
> nate resources
```

Generates and resizes icons and splash screens.

```
> nate update
```

Updates nate.

```
> nate verify
```

Verifies that the filesystem is correct and modules are installed.

```
nate build [ios or android]
```

Builds ios or android project add `--prod` or `-p` or `--production` for production.

```
> nate emulate [ios or android]
```

Opens device emulator.

```
> nate run [ios or android]
```

Runs on connected device.
