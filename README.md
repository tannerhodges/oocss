# OOCSS (VM-free version)

## Install Build Tools

```
cd tools && npm install
gem install compass
# Bonus: Mac Notifier
gem install terminal-notifier
```

## Build tasks

- `make build`
- `make watch`
- `make bw` - Runs `make build` and `make watch` at the same time.
- `make component -name [component name]` - Create a new component with the
  name you specify. E.g. `make component -name button`. This will
  automatically create the component folder, Sass, handlebar and JavaScript
  files.

## Directory Structure

- `src/`: SASS, handlebars, JavaScript, and JSON
- `build/`: Compile to CSS, HTML, and concatenated JavaScript

---

## How the build tasks work

Build:

```
# Runs clean first, then...
mkdir -p build/css
cd tools/config && compass compile
mkdir -p build/docs
node tools/build
```

Watch:

```
node tools/watch
```

Clean:

```
rm -rf build
rm -rf workshop*
cd tools/config && compass clean
```

Full reset:

```
rm -rf tools/node_modules
```
