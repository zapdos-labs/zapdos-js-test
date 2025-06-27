# zapdos-js-test

A simple test project for `zapdos-js`.

## Installation

```bash
npm install
```

`npm install` is necessary to set up the `node_modules` directory and install any other dependencies required by `zapdos-js-test`, even when `zapdos-js` is symlinked for local development.

## Usage

```bash
node index.js
```

## Local Development

To develop `zapdos-js` locally and test changes within `zapdos-js-test`, follow these steps:

1.  **Link `zapdos-js`:**
    Navigate to the `zapdos-js` directory:
    ```bash
    cd ../zapdos-js
    ```
    Then, create a global symlink for `zapdos-js`:
    ```bash
    npm link
    ```

2.  **Link `zapdos-js` in `zapdos-js-test`:**
    Navigate back to the `zapdos-js-test` directory:
    ```bash
    cd ../zapdos-js-test
    ```
    Then, link the globally installed `zapdos-js` to this project:
    ```bash
    npm link zapdos-js
    ```

Now, any changes you make in the `zapdos-js` directory will be reflected in `zapdos-js-test` without needing to reinstall.

To unlink the packages:

1.  In `zapdos-js-test` directory:
    ```bash
    npm unlink zapdos-js
    ```
2.  In `zapdos-js` directory:
    ```bash
    npm unlink
    ```

