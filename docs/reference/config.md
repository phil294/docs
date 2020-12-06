# Configuration

Here is the full options of `uvue.config.js` file

```js
export default {
  /**
   * Change default required paths
   */
  paths: {
    // Your main file with new Vue()
    main: './src/main.js',

    // Main template used for page rendering
    template: './src/index.html',
  },

  /**
   * Define UVue plugins
   */
  plugins: [
    // Use a plugin without options
    'some/plugin',

    // With some options
    ['some/plugin', { ...options }],
  ],

  /**
   * Imports some scripts in bundle
   */
  imports: [
    // Import script on both sides
    'some/path',

    // Import script only on client side
    ['some/path', { ssr: false }],
  ],

  /**
   * CSS management
   */
  css: {
    normal: 'inline', // Or `extract`
    vue: 'inline', // Or `extract`
  },
};
```
