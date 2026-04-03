[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/badge/#docusaurus_skipToContent_fallback)

On this page

Este componente é utilizado para informar status ou quantidade.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/badge/\#como-utilizar "Direct link to Como utilizar")

O badge é utilizado em situações em que seja necessário informar uma determinada quantidade de um item em listas, cadastros, cabeçalhos de modais, card, entre outros. Ele também é utilizado em diferentes situações, podendo ser diferenciado pela cor quando necessário.

Este componente também pode ser utilizado como tag (acompanhado por um × à direita do texto), ou como indicador de status.

- Exemplo
- Vanilla
- React
- Vue

45PagoEnviadoErroInconsistente [Opção 1×](https://docs.plataforma.betha.cloud/docs/design/componentes/badge/#)

```html
<span class="badge">45</span>
<span class="badge badge-success ml-1">Pago</span>
<span class="badge badge-info ml-1">Enviado</span>
<span class="badge badge-danger ml-1">Erro</span>
<span class="badge badge-warning ml-1">Inconsistente</span>
<a href="#" class="badge ml-1">Opção 1<span class="ml-2">&times;</span></a>
```

```html
<span className="badge">45</span>
<span className="badge badge-success ml-1">Pago</span>
<span className="badge badge-info ml-1">Enviado</span>
<span className="badge badge-danger ml-1">Erro</span>
<span className="badge badge-warning ml-1">Inconsistente</span>
<a href="#" className="badge ml-1">Opção 1<span className="ml-2">&times;</span></a>
```

```html
<b-badge pill variant="light">45</b-badge>
<b-badge pill variant="success">Pago</b-badge>
<b-badge pill variant="info">Enviado</b-badge>
<b-badge pill variant="danger">Erro</b-badge>
<b-badge pill variant="warning">Inconsistente</b-badge>
<b-badge href="#" variant="light">Opção 1<span class="ml-2">&times;</span></b-badge>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/badge/#como-utilizar)