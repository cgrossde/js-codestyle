# JS-Codestyle

Some convetions I started using with my JS code.

Add this to your `scripts` section in `package.json`:
  
    "lint": "(node_modules/jscs/bin/jscs -c .jscsrc --max-errors 10  --reporter console . || exit 0) && (node_modules/eslint/bin/eslint.js -c .eslintrc . || exit 0)"

Then run lint with `npm run lint`. You could also use Sublime Linter with the `eslint` and `jscs` linter plugins.
