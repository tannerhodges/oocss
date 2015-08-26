# OOCSS (VM-free version)

## Getting Started

### Install Build Tools

```
cd tools && npm install
gem install compass
# Bonus: Mac Notifier
gem install terminal-notifier
```

### Build The Docs

```
make build
```

Then open `build/template/template.html` in your browser.

## Making It Your Own

Edit the files in `src/`.

For example:

- Changing `[Client name]` in `src/includes/_headTemplate.handlebars` updates the library page title.
- Changing `OOCSS` in `src/includes/_header.handlebars` updates the library page's header text.

Use the other build tasks to create new components and update the library.

## Task List

- `make build`
- `make watch`
- `make bw` - Runs `make build` and `make watch` at the same time.
- `make component -name [component name]` - Create a new component with the
  name you specify. E.g. `make component -name button`. This will
  automatically create the component folder, Sass, handlebar and JavaScript
  files.
