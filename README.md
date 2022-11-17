# browserslist-config-design-italia

Configurazione condivisa di [Browserslist](https://github.com/ai/browserslist) secondo il [Manuale operativo di design](https://docs.italia.it/italia/designers-italia/manuale-operativo-design-docs/it/versione-corrente/doc/esperienza-utente/lo-sviluppo-della-interfaccia-utente.html#supporto-browser).

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
