[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#docusaurus_skipToContent_fallback)

On this page

Esta implementação estiliza o [Bootstrap 4](https://getbootstrap.com/docs/4.5/getting-started/introduction/) de acordo com a especificação do Design System Betha.

## GitHub [​](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/\#github "Direct link to GitHub")

Explore o projeto no GitHub [https://github.com/betha-plataforma/theme-bootstrap4](https://github.com/betha-plataforma/theme-bootstrap4)

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/\#como-utilizar "Direct link to Como utilizar")

É possível baixar o tema usando NPM ou Yarn, ou ainda referenciá-lo diretamente via CDN.

### NPM [​](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/\#npm "Direct link to NPM")

```shell
npm install @betha-plataforma/theme-bootstrap4
```

### Yarn [​](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/\#yarn "Direct link to Yarn")

```shell
yarn add @betha-plataforma/theme-bootstrap4
```

### CDN (unpkg) [​](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/\#cdn-unpkg "Direct link to CDN (unpkg)")

```html
<link rel="stylesheet" href="https://unpkg.com/@betha-plataforma/theme-bootstrap4">
```

## Pré-requisitos [​](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/\#pr%C3%A9-requisitos "Direct link to Pré-requisitos")

Além do [Bootstrap 4](https://getbootstrap.com/docs/4.5/getting-started/introduction/), este tema utiliza os ícones da biblioteca [Material Design Icons](https://cdn.materialdesignicons.com/5.4.55/). Observe a sequência em que essas dependências devem ser importadas:

```html
<html>
  <head>
    <!-- Bootstrap 4 e Material Design Icons -->
    <link rel="stylesheet" href="https://unpkg.com/bootstrap@4.5.2/dist/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://unpkg.com/@mdi/font@5.0.45/css/materialdesignicons.min.css">

    <!-- Tema para Bootstrap 4 -->
    <link rel="stylesheet" href="https://unpkg.com/@betha-plataforma/theme-bootstrap4">
  </head>
  <!-- ... -->
</html>
```

## Compatibilidade [​](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/\#compatibilidade "Direct link to Compatibilidade")

Este tema é compatível com as principais implementações do Bootstrap 4 para Angular, React e Vue. A seguir estão listadas as implementações compatíveis:

| Framework/Lib | Implementação compatível |
| --- | --- |
| Angular | [Ng-bootstrap](https://ng-bootstrap.github.io/#/getting-started) |
| React | [React Bootstrap](https://react-bootstrap.github.io/getting-started/introduction) |
| Vue | [BootstrapVue](https://bootstrap-vue.org/docs) |

Apenas os componentes especificados neste Design System foram estilizados e testados para as implementações listadas acima.

- [GitHub](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#github)
- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#como-utilizar)
  - [NPM](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#npm)
  - [Yarn](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#yarn)
  - [CDN (unpkg)](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#cdn-unpkg)
- [Pré-requisitos](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#pr%C3%A9-requisitos)
- [Compatibilidade](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4/#compatibilidade)