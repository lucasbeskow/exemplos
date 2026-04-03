[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/#docusaurus_skipToContent_fallback)

On this page

Você pode criar layouts com espaçamentos internos (padding) e externos (margin) entre os elementos.
Tanto a classe `.p-`, quanto a classe `.m-` possuem uma escala de 1 a 5, sendo 1 o menor e 5, o maior.

## Interno [​](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/\#interno "Direct link to Interno")

Você pode combinar a classe para determinar o nível de espaço com a direção:

- `.p-1` Todas as direções
- `.pt-1` Topo
- `.pr-1` Direita
- `.pb-1` Fundo
- `.pl-1` Esquerda

### Exemplo [​](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/\#exemplo "Direct link to Exemplo")

.p1

.pt-2 .pb-2 .pl-5 .pr-5

.pt-5 .p-2

- Vanilla

```html
<div class="container">
    <div class="row">
        <div class="col-12">
            <div class="p-1">...</div>
            <div class="pt-2 pb-2 pl-5 pr-5">...</div>
            <div class="pt-5 p-2">...</div>
        </div>
    </div>
</div>
```

## Externo [​](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/\#externo "Direct link to Externo")

Você pode combinar a classe para determinar o nível de espaço com a direção:

- `.m-1` Todas as direções
- `.mt-1` Topo
- `.mr-1` Direita
- `.mb-1` Fundo
- `.ml-1` Esquerda

### Exemplo [​](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/\#exemplo-1 "Direct link to Exemplo")

.m-1

.mt-2 .mb-2 .ml-5 .mr-5

.mt-5 .m-2

- Vanilla

```html
<div class="container">
    <div class="row">
        <div class="col-12">
            <div class="m-1">...</div>
            <div class="mt-2 mb-2 ml-5 mr-5">...</div>
            <div class="mt-5 m-2">...</div>
        </div>
    </div>
</div>
```

Para opções mais avançadas de espaçamento, consulte a documentação do [Bootstrap 4](https://getbootstrap.com/docs/4.6/utilities/spacing/).

- [Interno](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/#interno)
  - [Exemplo](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/#exemplo)
- [Externo](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/#externo)
  - [Exemplo](https://docs.plataforma.betha.cloud/docs/design/layout/espacamento/#exemplo-1)