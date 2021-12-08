# Azury's Bundler

> [`@azury/bundler`](https://npm.im/@azury/bundler) was primarily created for **Azury's projects** and might not work for yours.

### Installation

Install the package using your favorite package manager.

```sh-session
npm i @azury/bundler
yarn add @azury/bundler
```

### Usage

Build `src/index.js` in watch mode and save the bundled file as `build/index.js`.

```sh-session
build -i src/index.js -o build/index.js -w
```

## Bundle Mode

Bundles a specific file using **esbuild**.

```sh-session
build
```

### Define Input and Output

```sh-session
build --input src/index.js --output build/index.js
```
```sh-session
build -i src/index.js -o build/index.js
```

### Bundle in Watch Mode

```sh-session
build --watch
```
```sh-session
build -w
```

### Bundle CSS Modules

```sh-session
build --css
```
```sh-session
build -css
```

### Bundle to ESM

```sh-session
build --esm
```
```sh-session
build -esm
```

## Minify Mode

```sh-session
build minify
```

### Define Input and Output

Both can be either a directory or file.

```sh-session
build minify --input myfile.js --output myfile.min.js
```
```sh-session
build minify -i myfile.js -o myfile.min.js
```

## ZIP Mode

```sh-session
build zip
```

### Define Files to Include

```sh-session
build zip --files some.png other.png image.png
```
```sh-session
build zip -f some.png other.png image.png
```

### Define Output ZIP

```sh-session
build zip --output myarchive.zip
```
```sh-session
build zip -o myarchive.zip
```


