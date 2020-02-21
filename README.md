# ammuench TS Template

My base template for starting a TS app

## Tools

### Yarn

This repo is built using `yarn` instead of the standard `npm`. You can manually replace all instances of `yarn` in `package.json` with `npm run` and it should convert over no problem.

### Typescript

This repo uses the latest version of Typescript 3.8.

### Mocha, Chai, Sinon, NYC

This repo uses Mocha, Chai, and Sinon for testing. It uses NYC for testing code coverage. All tests should exist in the `test/` folder, and files should follow the pattern `**.spec.ts`. For example, if you have a file named `myfile.ts` in `src/`, then you should have an equivalent `myfile.spec.ts` for testing in the `test/` folder.

### Husky, Prettier, and Pretty-Quick support

Out of the box, this has been configured with `husky` for git hook support on commit and push.

On commit, we use `prettier` and `pretty-quick` to lint and fix all files staged for commit. This will check all staged files for linting, and fix them where possible before beginning the commit. This can be bypasses with the `--no-verify` flag when committing.

On push we run and make sure that all tests pass. This can be bypasses with the `--no-verify` flag when pushing.

## Commands

**yarn build**

> Builds the project and outputs the built files to the `/dist` folder

**yarn build:watch**

> Builds the project and outputs the built files to the `/dist` folder. Watches for changes and rebuilds every time change is detected

**yarn coverage**

> Runs unit tests and provides a report of the level of code coverage for all files in `/src/`

**yarn lint**

> Runs `prettier` on the root directory, and attempts to fix all files

**yarn test**

> Runs all unit tests in the `/tests/` folder

**yarn test:watch**

> Runs all unit tests in the `/tests/` folder. Watches for changes and re-runs tests every time change is detected

**yarn start**

> Runs `/dist/index.js` from the build output folder
