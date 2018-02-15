---
title: Плагины для wepback
description: Как добавить плагины для webpack в мое Nuxt.js приложение?
---

# Как добавить плагины для webpack?

In your `nuxt.config.js` file:

```js
const webpack = require('webpack')

module.exports = {
  build: {
    plugins: [
      new webpack.ProvidePlugin({
        '$': 'jquery',
        '_': 'lodash'
        // ...etc.
      })
    ]
  }
}
```
