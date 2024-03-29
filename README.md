# Development

This file describes steps for installing and developing the website locally.
The end of the file describes the different technologies and frameworks used.

## Mac Installation of Node v18

1. Install Homebrew, a terminal-based package manager. If you haven't yet
    installed Homebrew, you can do so [here](https://brew.sh/).
2. Run `brew update` to update Homebrew.
3. Run `brew install node@18`.
4. Check that you have both `node` and `npm` installed by running

        node -v
        npm -v

## Setting Up Local Development Environment

**All commands should be run in the `src/` directory.**

Install `npm` packages:

        npm install

To start the server on a local port, run

        npm run build
        npm run start

Then, in your browser, go to the localhost URL printed in the terminal.

Alternatively, if you would like to have the browser automatically refresh
when you save changes to React components and `server.js`, instead run

        npm run watch

Then, go to the **Loopback** URL, **not** the URL following `nodemon` output.

## Different Technologies Used
Name | Description
--- | ---
Babel | A Javascript and Typescript transpiler that allows compatibility with older environments if language features are not supported natively. Babel also helps transpile JSX/TSX syntax and React components to browser-supported JavaScript.
Node | Node(.js) is a cross-platform server environment that supports   JavaScript outside of the browser.
React | React(.js) is a JavaScript framework for building UI/UX interfaces via individual pieces called components.
Typescript | TypeScript is a superset of JavaScript that adds static typing.
webpack | webpack is a module bundler for JavaScript that turns a JavaScript module into a static, self-contained package with all necessary dependent modules.

