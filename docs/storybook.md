# Storybook

[todo]

# Configuring Storybook

You can configure storybook by adding a `storybook.main.js` file to your `web/config` directory (note that this directory may or may not exist&mdash;i.e. you might have to create it):

```js
// web/src/config/storybook.main.js

module.exports = {
  addons: ['@storybook/a11y-addon']
}
```

This file should return an object; this object will be merged with Redwood's base configuration, which you can find here: https://github.com/redwoodjs/redwood/blob/main/packages/core/config/storybook/main.js

Note that there's two files for configuring storybook: the `storybook.main.js` file and the `storybook.preview.js` file. They're for different things. If you want to add a decorator, do it in the `.preview.js` file. If you want to add a plugin, do it in `.main.js`.

# Other sections

[todo]

- link to mocking graphql requests
- link to or rehash some of the tutorial
- some storybook 101