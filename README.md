# vuepress-plugin-reading-progress

> plugin for vuepress

[README](README.md) | [CHANGELOG](CHANGELOG.md)

**This plugin is for Vuepress 1.x which is currently in alpha**

add reading progress bar for vuepress

---

## Installation

``` sh
yarn add vuepress-plugin-reading-progress
// or
npm i vuepress-plugin-reading-progress
```

## Usage

``` js
module.exports = {
  plugins: [
    'reading-progress'
  ]
}
```

[ Vuepress documentation](https://v1.vuepress.vuejs.org/plugin/using-a-plugin.html)


## Options

### readingDir
- Type: `null`, `string`, `array`, `Object`
- Default: `null`

Specify folders that display reading progress bar

example
``` js
{
  readingDir: 'posts'
  // or
  readingDir: ['posts1', 'posts2', 'posts3']
  // or { dir: fixed }
  readingDir: {
    posts1: 'top',
    posts2: 'bottom',
    posts3: 'top'
  }
}
```

### fixed
- Type: `string`
- Default: `top`

support `top`, `bottom`

set position for reading progress bar

## style

If you wish to apply simple color overrides to the styling

```
+- .vuepress
  +- styles
    +- palette.styl
```

``` css
$readingBgColor = transparent
$readingZIndex = 1000
$readingHeight = 3px
$readingProgressColor = $accentColor
```

## License

[MIT](http://opensource.org/licenses/MIT)

## Keywords

vue vuepress plugin reading-progress vreading progress
