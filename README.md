# JS-Codestyle

Some convetions I started using with my JS code.

Add `.eslintrc` and `.jscsrc` to your project root and install `eslint` and `jscs` as dev-dependecies to your `package.json`:

    npm install eslint jscs --save-dev

Then add this to your `scripts` section in `package.json`:

    "lint": "(node_modules/jscs/bin/jscs -c .jscsrc --max-errors 10  --reporter console . || exit 0) && (node_modules/eslint/bin/eslint.js -c .eslintrc . || exit 0)"

You can now lint your project with `npm run lint`. The SuplimeLinter plugin also supports `eslint` and `jscs`.
