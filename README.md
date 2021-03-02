# Presentation Template

Edit `index.html` to customize the presentation.  The presentation template
demonstrates basic concepts.  Much more can be found in the `examples` directory
and the reveal.js [documentation](https://revealjs.com/).

# Build and Package

After installing dependencies, either serve the presentation locally via the
built-in http server or build the presentation into a static website that
can be opened without running a server.

## Install dependencies

```bash
npm install
```

## Serve locally

```bash
npm start
```

This starts a webserver listening at http://0.0.0.0:8000.

## Build distribution

```bash
npx gulp package
```

This creates a file in the project base directory named `presentation.zip`.
This archive contains the presentation static assets within a base directory
named `presentation`.  To view the presentation, simply unzip the archive and
open `presentation/index.html` in a web browser.

### Note regarding the included build script

`package.json` contains a `build` script that consolidates JavaScript, CSS, and
any plugins into the `dist` directory before running tests.  This script should
not be used as it does not actualy result in the production of a usable
production archive.  Further, tests do not execute properly on various platforms
including WSL2.

# References

1. [reveal.js documentation](https://revealjs.com/)
