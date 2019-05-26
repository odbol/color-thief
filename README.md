# Color Thief

A script for grabbing the color palette from an image. Uses Javascript and the canvas tag to make it happen.

[See a Demo](http://lokeshdhakar.com/projects/color-thief) | [Read more on my blog](http://lokeshdhakar.com/color-thief)


## How to use

### Get the dominant color from an image

```js
var colorThief = new ColorThief();
colorThief.getColor(sourceImage);
```

### Build a color palette from an image

In this example, we build an 8 color palette.

```js
var colorThief = new ColorThief();
colorThief.getPalette(sourceImage, 8);
```

### API

| Method | Return | Description |
| --- | --- | --- |
| `getColor(image [, quality])` | `[Number, Number, Number]` | WIP |
| `getPalette(image [, colorCount, quality]` | `[[Number, Number, Number], ...]` | WIP |

---


## Contributing

### Running tests

Run Cypress integration tests in Chrome browser.

- `npm run dev` to start local server.
- `npm run test-browser`

Run node tests.
- `npm run test-node`

## Add tests

To add in browser tests:

- Update `index.html` if you need to add additional examples
- Add new tests in `cypress/integration/apis_spec.js`

To add node tests:

- Update `test/node-test.js`


### Making a new release

- Update version number in `src/color-thief.js` and `package.json`
- Run `npm run build`
- Push to Github repo
- Create a new Github release along with tag. Naming convention for both ```v2.8.1```
