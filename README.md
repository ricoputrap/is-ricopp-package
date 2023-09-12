# is-ricopp-package

This is a simple repository for learning how to create an NPM package.

### How to test the NPM package?
1. Navigate to the root directory of this project.
2. Run the following command:
    ```bash
    npm link
    ```
    This will make your package available globally in your computer.
3. Create a new folder outside this project and navigate to it. Let's say you name it as `test-folder`.
4. Run the following command:
    ```bash
    npm link is-ricopp
    ```
    This will generate a `node_modules` folder inside `test-folder`.
5. Add a new JS file (`script.js`) inside this `test-folder`. Write a few lines of code as follows:
    ```javascript
    const isRicoPP = require('is-ricopp');

    console.log(isRicoPP('RicoPP')); // return true
    console.log(isRicoPP('Rico PP')); // return false
    ```
6. Execute the following command:
    ```bash
    node script.js
    ```
    You should see the following output:
    ```bash
    true
    false
    ```


### Referrences
[How to Create and Publish an NPM Package – a Step-by-Step Guide](https://www.freecodecamp.org/news/how-to-create-and-publish-your-first-npm-package/)