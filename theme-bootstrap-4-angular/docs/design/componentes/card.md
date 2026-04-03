[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/card/#docusaurus_skipToContent_fallback)

On this page

Este componente tem o objetivo de agrupar dados que tenham relação direta entre si e de separar graficamente o conteúdo de uma interface.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/card/\#como-utilizar "Direct link to Como utilizar")

Sempre que for necessário apresentar conteúdo em um ambiente do sistema. Existem 3 variações do componente card: principal, com borda e com preenchimento.

### Card principal [​](https://docs.plataforma.betha.cloud/docs/design/componentes/card/\#card-principal "Direct link to Card principal")

Este card é utilizado diretamente sobre o background da aplicação. Nele são apresentados os conteúdos da interface. Não há limite de cards principais a serem utilizados numa mesma tela, desde que o conteúdo a ser demonstrado em cada um deles represente um grupo de informações relevantes ao usuário no ambiente em que estiverem sendo exibidas.

### Card com borda [​](https://docs.plataforma.betha.cloud/docs/design/componentes/card/\#card-com-borda "Direct link to Card com borda")

Este é um card secundário, utilizado para dividir conteúdos em um card principal. Ele serve de container para informações que pertençam a um mesmo grupo.

### Card com preenchimento [​](https://docs.plataforma.betha.cloud/docs/design/componentes/card/\#card-com-preenchimento "Direct link to Card com preenchimento")

Esta é uma outra opção de card secundário. Também deve ser utilizado com a mesma finalidade do card com borda, porém recomenda-se o uso de apenas um card com preenchimento por card principal já que esse componente tem o objetivo de destacar um grupo de informações, transmitindo a ideia de que esse grupo destacado tem maior importância em relação aos demais.

- Vanilla

```html
<!-- Card básico -->
<div class="card border-0">
    <div class="card-body">
        Conteúdo do card básico
    </div>
</div>

<!-- Card com borda -->
<div class="card">
    <div class="card-body">
        Conteúdo do card com borda
    </div>
</div>

<!-- Card com preenchimento -->
<div class="card border-0 bg-secondary">
    <div class="card-body">
        Conteúdo do card com preenchimento
    </div>
</div>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/card/#como-utilizar)
  - [Card principal](https://docs.plataforma.betha.cloud/docs/design/componentes/card/#card-principal)
  - [Card com borda](https://docs.plataforma.betha.cloud/docs/design/componentes/card/#card-com-borda)
  - [Card com preenchimento](https://docs.plataforma.betha.cloud/docs/design/componentes/card/#card-com-preenchimento)