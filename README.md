# OOCSS (forked)

## Install

```
vagrant up
vagrant ssh
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
