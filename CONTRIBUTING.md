# Contributing

This document describes how to contribute to Batarang

## Installing from Source

1. Clone the repository: `git clone git@github.com:angular/batarang.git`
2. Install the npm dependencies `yarn install`
3. Build the inject script: `yarn build`
4. Navigate to `chrome://extensions` and enable Developer Mode.
5. Choose "Load unpacked extension"
6. In the dialog, open the directory you just cloned.

## Running the tests

- To run the tests once: `yarn test`
- To watch the directory, running tests whenver something is updated: `yarn test:watch`

## Creating a PR

Please follow the code & commit guidelines found in [Angular core's CONTRIBUTING.md](https://github.com/angular/angular.js/blob/master/CONTRIBUTING.md#submitting-a-pull-request).

## Packaging a release

I (@btford) will do this periodically, but I'm adding these instructions here
for posterity.

1. Edit the version number in `manifest.json` and `package.json` with the new version.
2. Run `gulp zip`
3. `git add package.json manifest.json dist/`
4. `git commit -m "v1.2.3"`
5. `git tag v1.2.3`
6. `git push upstream master && git push upstream --tags`
7. Upload `batarang-v1.2.3.zip` to Web Store via the [Web Store Dashboard](https://chrome.google.com/webstore/developer/dashboard)

## Layout

The `panel` directory contains...
`panel/components` contains self-contained directives and services.

## Testing Batarang manually


