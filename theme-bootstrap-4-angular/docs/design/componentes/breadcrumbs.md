[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/breadcrumbs/#docusaurus_skipToContent_fallback)

On this page

Este componente é utilizado para demonstrar uma estrutura de navegação que representa o caminho percorrido no sistema para o acesso à funcionalidade que está sendo exibida no momento.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/breadcrumbs/\#como-utilizar "Direct link to Como utilizar")

Caminhos não navegáveis não são clicáveis; já em páginas navegáveis, utiliza-se o link para acesso rápido ao conteúdo. A página atual nunca será clicável, é apenas informativa.

- Exemplo
- Vanilla
- React
- Vue

```html
<nav aria-label="breadcrumb">
  <ol class="breadcrumb">
    <li class="breadcrumb-item"><a href="#">Grupo</a></li>
    <li class="breadcrumb-item"><a href="#">Subgrupo</a></li>
    <li class="breadcrumb-item active" aria-current="page">Item</li>
  </ol>
</nav>
```

```html
<Breadcrumb>
  <Breadcrumb.Item href="#">Grupo</Breadcrumb.Item>
  <Breadcrumb.Item href="#">Subgrupo</Breadcrumb.Item>
  <Breadcrumb.Item active>Item</Breadcrumb.Item>
</Breadcrumb>
```

```html
<b-breadcrumb :items="items"></b-breadcrumb>

<script>
  export default {
    data() {
      return {
        items: [\
          {\
            text: 'Grupo',\
            href: '#'\
          },\
          {\
            text: 'Subgrupo',\
            href: '#'\
          },\
          {\
            text: 'Item',\
            active: true\
          }\
        ]
      }
    }
  }
</script>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/breadcrumbs/#como-utilizar)