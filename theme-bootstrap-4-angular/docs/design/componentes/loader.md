[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/loader/#docusaurus_skipToContent_fallback)

On this page

Loader é um indicador de carregamento cujo objetivo é transmitir ao usuário a informação de que o sistema precisa de algum tempo para processar as informações solicitadas, seja o carregamento de uma página ou a execução de um processo, por exemplo.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/loader/\#como-utilizar "Direct link to Como utilizar")

Este componente deve ser utilizado em qualquer situação onde seja necessário dar feedback ao usuário de que um processo em segundo plano está sendo executado e que ele deve aguardar o término dessa operação, seja no carregamento de um ambiente por inteiro ou em partes da interface.

- Exemplo
- Vanilla
- React

```html
<div class="d-flex justify-content-center align-items-center">
    <div class="spinner-grow" role="status"></div>
</div>
```

```html
<div className="spinner-grow"></div>
```

### Variação de tamanho [​](https://docs.plataforma.betha.cloud/docs/design/componentes/loader/\#varia%C3%A7%C3%A3o-de-tamanho "Direct link to Variação de tamanho")

Este componente também pode ser exibido _inline_, como no exemplo a seguir, em que o clique no botão dispara uma ação assíncrona e demonstra ao usuário que o resultado está sendo carregado. Neste caso, utiliza-se a classe `.spinner-grow-sm` para reduzir o tamanho do componente afim de utilizá-lo junto ao texto.

- Exemplo
- Vanilla
- React

Botão

```html
<span class="spinner-grow spinner-grow-sm mr-3" role="status"></span>
```

```html
<Button size="sm" variant="secondary"><span className="spinner-grow spinner-grow-sm mr-3"></span>Botão</Button>
```

### Loader com backdrop [​](https://docs.plataforma.betha.cloud/docs/design/componentes/loader/\#loader-com-backdrop "Direct link to Loader com backdrop")

Nos casos em que a interface ou bloco ainda não estiverem prontos para que o usuário possa interagir com seu conteúdo, recomenda-se o uso do loader com backdrop. Neste caso, o componente ocupará a largura e a altura totais do container que possuir a propriedade CSS `position: relative`.

Para garantir que o backdrop ocupe a largura e a altura totais da página, é possível combinar a classe `spinner-grow-backdrop` com a classe auxiliar do Bootstrap 4 `position-fixed`.

- Exemplo
- Vanilla
- React

```html
<div class="spinner-grow-backdrop">
    <div class="spinner-grow"></div>
</div>
```

```html
<div className="spinner-grow-backdrop">
    <div className="spinner-grow"></div>
</div>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/loader/#como-utilizar)
  - [Variação de tamanho](https://docs.plataforma.betha.cloud/docs/design/componentes/loader/#varia%C3%A7%C3%A3o-de-tamanho)
  - [Loader com backdrop](https://docs.plataforma.betha.cloud/docs/design/componentes/loader/#loader-com-backdrop)