# browserslist-config-design-italia

Configurazione condivisa di [Browserslist](https://github.com/ai/browserslist) secondo le [Linee Guida di Design per i servizi web della Pubblica Amministrazione, sezione 6.3.1.2.1. Supporto browser](https://docs.italia.it/italia/designers-italia/design-linee-guida-docs/it/2020.1/doc/user-interface/lo-sviluppo-di-un-interfaccia-e-i-web-kit.html#strumenti).

```sh
yarn add --dev browserslist-config-design-italia
```

## Utilizzo

Se vuoi utilizzare questo pacchetto in un'applicazione, aggiungi questa configurazione al `package.json`:

```js
{
    "browserslist": [
        "extends browserslist-config-design-italia"
    ]
}
```

Se vuoi configurare manualmente uno strumento che utilizza Browserslist, poi importare questo pacchetto per ottenere una lista di browser supportati.

Ad esempio configurando [@babel/preset-env](https://babeljs.io/docs/en/babel-preset-env) via JavaScript:

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

### Licenza

BSD-3-Clause