# browserslist-config-design-italia

[![Versione](https://img.shields.io/npm/v/browserslist-config-design-italia.svg?logo=npm)](https://github.com/italia/browserslist-config-design-italia/releases)
[![GitHub issues](https://img.shields.io/github/issues/italia/browserslist-config-design-italia.svg)](https://github.com/italia/browserslist-config-design-italia/issues)
[![Join the #design channel](https://img.shields.io/badge/Slack%20channel-%23design-blue.svg)](https://developersitalia.slack.com/messages/C7VPAUVB3/)
[![Get invited](https://slack.developers.italia.it/badge.svg)](https://slack.developers.italia.it/)

Shareable [Browserslist](https://github.com/ai/browserslist) configuration following the [Linee Guida di Design per i servizi web della Pubblica Amministrazione, sezione 6.3.1.2.1. Supporto browser](https://docs.italia.it/italia/designers-italia/design-linee-guida-docs/it/2020.1/doc/user-interface/lo-sviluppo-di-un-interfaccia-e-i-web-kit.html#strumenti).

```sh
yarn add --dev browserslist-config-design-italia
```

## Usage

If you want to use this package within your application, add these lines to the `package.json`:

```js
{
    "browserslist": [
        "extends browserslist-config-design-italia"
    ]
}
```

If you want to manually configure a tool that uses Browserslist, importing this package returns the array of supported browsers.

For example, when configuring [@babel/preset-env](https://babeljs.io/docs/en/babel-preset-env) via JavaScript:


```js
{
  presets: [
    ['env', {
      targets: {
        browsers: require('browserslist-config-design-italia')
      }
    }]
  ]
}
```

### License

BSD-3-Clause