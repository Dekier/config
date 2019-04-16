# config

Add libraries to project: 

* eslint
* eslint-config-prettier
* eslint-config-standard
* eslint-loader
* eslint-plugin-import
* eslint-plugin-jest
* eslint-plugin-node
* eslint-plugin-nuxt
* eslint-plugin-prettier
* eslint-plugin-promise
* eslint-plugin-standard
* eslint-plugin-vue
* prettier

Add rules for settings in **Visual Studio Code:**

```  "eslint.enable": true,
    "eslint.run": "onType",
    "eslint.validate": [
        {
            "language": "vue",
            "autoFix": true
        },
        {
            "language": "html",
            "autoFix": true
        },
        {
            "language": "javascript",
            "autoFix": true
        },
        {
            "language": "javascriptreact",
            "autoFix": true
        }
    ],
    "eslint.alwaysShowStatus": true,
    "eslint.autoFixOnSave": true,
    "vetur.format.defaultFormatter.js": "prettier",
    "vetur.format.defaultFormatter.html": "prettier",
    "vetur.format.defaultFormatter.css": "prettier",
    "editor.formatOnSave": true
```
    
**.eslintrc.js:

```module.exports = {
  root: true,
  env: {
    browser: true,
    node: true
  },
  parserOptions: {
    parser: 'babel-eslint'
  },
  extends: [
    '@nuxtjs',
    'plugin:nuxt/recommended',
    'plugin:prettier/recommended',
    'prettier',
    'prettier/vue'
  ],
  plugins: [
    'prettier',
    'vue'
  ],
  // add your custom rules here
  rules: {
  }
}
```

**.prettierrc.json

```{
  "jsxSingleQuote": true,
  "printWidth": 80,
  "singleQuote": true,
  "tabWidth": 2,
  "useTabs": false,
  "semi": false,
  "bracketSpacing": true,
  "arrowParens": "always",
  "trailingComma": "es5",
  "jsxBracketSameLine": true
}
```
