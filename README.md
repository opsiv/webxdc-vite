# WebXDC Vite Template [![CI](https://github.com/webxdc/webxdc-vite/actions/workflows/ci.yml/badge.svg)](https://github.com/webxdc/webxdc-vite/actions/workflows/ci.yml) [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)

A minimalist Vite project template for WebXDC development.

## Features

- ⚡️ Fast development with [Vite](https://github.com/vitejs/vite) and [pnpm](https://pnpm.js.org/)

- 📱 Integrated [WebXDC emulator](https://github.com/webxdc/webxdc-dev) to test your WebXDC right on the browser while developing,
  and [Eruda](https://github.com/liriliri/eruda) to debug inside Delta Chat.

- ✅ Use [Vitest](http://vitest.dev/) for unit testing

- 📝 Code formatting with [Prettier](https://github.com/prettier/prettier)

- 📦 Automatically minify, build and release your `.xdc` file

## Usage

### Installing Dependencies

After cloning this repo for the first time, install dependecies:

```
pnpm i
```

### Running tests

```
pnpm test
```

### Testing the app in the browser

To test your work in your browser (with hot reloading!) while developing:

```
pnpm dev-mini
# Alternatively to test in a more advanced WebXDC emulator:
npm run dev
```

**💡 TIP:** To debug inside Delta Chat, uncomment the `script` tag at the end of
`index.html` file and your WebXDC will be packaged with developer tools inside!

### Building

To package your WebXDC file:

```
pnpm build
```

The resulting optimized `.xdc` file is saved in `dist/` folder.

### Releasing

To automatically build and create a new GitHub release with your `.xdc` file:

```
git tag v1.0.1
git push origin v1.0.1
```

## Try it now!

[**Create a repo from this template on GitHub**](https://github.com/webxdc/webxdc-vite/generate).
