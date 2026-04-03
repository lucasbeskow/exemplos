[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/popover/#docusaurus_skipToContent_fallback)

On this page

Popovers são containers que se abrem sobre o conteúdo principal para a exibição de uma funcionalidade complementar.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/popover/\#como-utilizar "Direct link to Como utilizar")

Este componente é utilizado para simplificar a inserção e visualização de dados. Seu objetivo é possibilitar trabalhar com campos, texto e outros elementos sobre uma interface. Os popovers permitem acessar detalhes ou ações de seus dados sem ter que sair do ambiente, mantendo o contexto da interface.

São quatro posições de exibição possíveis em relação ao elemento que dá acesso a esse componente: superior, inferior, esquerda e direita, conforme demonstrado abaixo.

- Exemplo
- Vanilla
- Angular
- React
- Vue

Abrir à esquerdaAbrir acimaAbrir abaixoAbrir à direita

```html
<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="left" data-content="Conteúdo do popover" data-title="Título do popover">
  Abrir à esquerda
</button>
<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="top" data-content="Conteúdo do popover" data-title="Título do popover">
  Abrir acima
</button>
<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="bottom" data-content="Conteúdo do popover" data-title="Título do popover">
  Abrir abaixo
</button>
<button type="button" class="btn btn-secondary" data-container="body" data-toggle="popover" data-placement="right" data-content="Conteúdo do popover" data-title="Título do popover">
  Abrir à direita
</button>
```

```html
<button type="button" class="btn btn-secondary" placement="left" ngbPopover="Conteúdo do popover" popoverTitle="Título do popover">
  Abrir à esquerda
</button>
<button type="button" class="btn btn-secondary" placement="top" ngbPopover="Conteúdo do popover" popoverTitle="Título do popover">
  Abrir acima
</button>
<button type="button" class="btn btn-secondary" placement="bottom" ngbPopover="Conteúdo do popover" popoverTitle="Título do popover">
  Abrir abaixo
</button>
<button type="button" class="btn btn-secondary" placement="right" ngbPopover="Conteúdo do popover" popoverTitle="Título do popover">
  Abrir à direita
</button>
```

```html
<>
  {['top', 'right', 'bottom', 'left'].map((placement) => (
    <OverlayTrigger
      trigger="click"
      key={placement}
      placement={placement}
      overlay={
        <Popover id={`popover-positioned-${placement}`}>
          <Popover.Title as="h3">{`Popover ${placement}`}</Popover.Title>
          <Popover.Content>
            <strong>Holy guacamole!</strong> Check this info.
          </Popover.Content>
        </Popover>
      }
    >
      <Button variant="secondary">Popover on {placement}</Button>
    </OverlayTrigger>
  ))}
</>
```

```html
<b-button v-b-popover.click.left="'Conteúdo do popover'" title="Título do popover">
    Abrir à esquerda
</b-button>
<b-button v-b-popover.click.top="'Conteúdo do popover'" title="Título do popover">
    Abrir acima
</b-button>
<b-button v-b-popover.click.bottom="'Conteúdo do popover'" title="Título do popover">
    Abrir abaixo
</b-button>
<b-button v-b-popover.click.right="'Conteúdo do popover'" title="Título do popover">
    Abrir à direita
</b-button>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/popover/#como-utilizar)