[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/#docusaurus_skipToContent_fallback)

On this page

As classes `.row` possuem comportamento flexível, portanto, podem utilizar as classes de alinhamento nas divs filhas. Caso a div não possua essa classe, você poderá adicionar a classe `.d-flex` para que ela tenha o mesmo comportamento.

## Vertical [​](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/\#vertical "Direct link to Vertical")

Utilize as classes com `.row` ou `.d-flex`:

`.align-items-start` para alinhar no início (topo)

Div 1

Div 2

Div 3

`.align-items-center` para alinhar no meio

Div 1

Div 2

Div 3

`.align-items-end` para alinhar no fim (fundo)

Div 1

Div 2

Div 3

### Exemplo [​](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/\#exemplo "Direct link to Exemplo")

- Vanilla

```html
<div class="container">
    <div class="row align-items-center">
        <div class="col-12 col-sm-6 col-lg-4">Div 1</div>
        <div class="col-12 col-sm-6 col-lg-4">Div 2</div>
        <div class="col-12 col-sm-6 col-lg-4">Div 3</div>
    </div>
</div>
```

## Horizontal [​](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/\#horizontal "Direct link to Horizontal")

Utilize as classes com `.row` ou `.d-flex`:

`.justify-content-start` para alinhar no início da linha

Div 1

Div 2

Div 3

`.justify-content-center` para alinhar no meio da linha

Div 1

Div 2

Div 3

`.justify-content-end` para alinhar no fim da linha

Div 1

Div 2

Div 3

### Exemplo [​](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/\#exemplo-1 "Direct link to Exemplo")

- Vanilla

```html
<div class="container">
    <div class="row justify-content-center">
        <div class="col-12 col-sm-6 col-lg-4">Div 1</div>
        <div class="col-12 col-sm-6 col-lg-4">Div 2</div>
        <div class="col-12 col-sm-6 col-lg-4">Div 3</div>
    </div>
</div>
```

Para opções mais avançadas de alinhamento, consulte a documentação do [Bootstrap 4](https://getbootstrap.com/docs/4.6/utilities/flex/#align-items).

- [Vertical](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/#vertical)
  - [Exemplo](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/#exemplo)
- [Horizontal](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/#horizontal)
  - [Exemplo](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento/#exemplo-1)