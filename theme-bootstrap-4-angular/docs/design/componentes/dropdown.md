[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/dropdown/#docusaurus_skipToContent_fallback)

On this page

Este componente tem o objetivo de exibir um menu suspenso com uma lista de opções.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/dropdown/\#como-utilizar "Direct link to Como utilizar")

Quando for necessário apresentar uma lista de opções que não ocupe espaço na interface principal, sendo exibida apenas com a intervenção do usuário.

- Exemplo
- Vanilla
- Angular
- React
- Vue

Opções

Opções

Opções

Opções

Opções

Opções

```html
<div class="dropdown">
  <button class="btn btn-secondary dropdown-toggle" type="button" id="dropdownMenuButton"
    data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
    Opções
  </button>
  <div class="dropdown-menu" aria-labelledby="dropdownMenuButton">
    <h6 class="dropdown-header">Título do dropdown</h6>
    <a class="dropdown-item" href="#">Opção 1</a>
    <a class="dropdown-item" href="#">Opção 2</a>
    <div class="dropdown-divider"></div>
    <a class="dropdown-item" href="#">Opção 3</a>
  </div>
</div>
```

```html
<div ngbDropdown class="d-inline-block">
    <button class="btn btn-secondary" id="dropdownBasic1" ngbDropdownToggle>Opções</button>
    <div ngbDropdownMenu aria-labelledby="dropdownBasic1">
        <h6 class="dropdown-header">Título do dropdown</h6>
        <button ngbDropdownItem>Opção 1</button>
        <button ngbDropdownItem>Opção 2</button>
        <div class="dropdown-divider"></div>
        <button ngbDropdownItem>Opção 3</button>
    </div>
</div>
```

```html
<Dropdown>
  <Dropdown.Toggle variant="secondary" size="sm">
    Opções<i className="mdi mdi-chevron-down ml-1"></i>
  </Dropdown.Toggle>
  <Dropdown.Menu>
    <Dropdown.Header>Título do dropdown</Dropdown.Header>
    <Dropdown.Item href="#">Opção 1</Dropdown.Item>
    <Dropdown.Item href="#">Opção 2</Dropdown.Item>
    <Dropdown.Divider />
    <Dropdown.Item href="#">Opção 3</Dropdown.Item>
  </Dropdown.Menu>
</Dropdown>
```

```html
<b-dropdown text="Opções" class="m-2">
    <b-dropdown-group id="dropdown-group-1" header="Título do dropdown">
        <b-dropdown-item-button>Opção 1</b-dropdown-item-button>
        <b-dropdown-item-button>Opção 2</b-dropdown-item-button>
        <b-dropdown-divider></b-dropdown-divider>
        <b-dropdown-item-button>Opção 3</b-dropdown-item-button>
    </b-dropdown-group>
</b-dropdown>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/dropdown/#como-utilizar)