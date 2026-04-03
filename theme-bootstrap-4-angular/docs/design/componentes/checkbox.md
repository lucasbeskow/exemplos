[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/checkbox/#docusaurus_skipToContent_fallback)

On this page

Este componente permite marcar um ou mais itens de uma lista de opções.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/checkbox/\#como-utilizar "Direct link to Como utilizar")

Sempre que houver a necessidade de marcar uma ou mais opções, bem como fazer uma seleção em lote em uma lista de itens. Ele pode ser utilizado individualmente, em listas, ou inserido em tabelas.

### Formato horizontal [​](https://docs.plataforma.betha.cloud/docs/design/componentes/checkbox/\#formato-horizontal "Direct link to Formato horizontal")

- Exemplo
- Vanilla
- React
- Vue

Opção 1

Opção 2

Opção 3

```html
<div class="form-check form-check-inline">
    <input class="form-check-input" type="checkbox" id="chbxh1" value="1">
    <label class="form-check-label" for="chbxh1">Opção 1</label>
</div>
<div class="form-check form-check-inline">
    <input class="form-check-input" type="checkbox" id="chbxh2" value="2">
    <label class="form-check-label" for="chbxh2">Opção 2</label>
</div>
<div class="form-check form-check-inline">
    <input class="form-check-input" type="checkbox" id="chbxh3" value="3" disabled>
    <label class="form-check-label" for="chbxh3">Opção 3</label>
</div>
```

```html
<Form>
    <Form.Group>
        <Form.Check type="checkbox" label="Opção 1" inline id="chbxh1" />
        <Form.Check type="checkbox" label="Opção 2" inline id="chbxh2" />
        <Form.Check type="checkbox" label="Opção 3" inline id="chbxh3" disabled />
    </Form.Group>
</Form>
```

```html
<b-form-group>
    <b-form-checkbox-group v-model="selected" :options="options" name="chbxh"></b-form-checkbox-group>
</b-form-group>
```

### Formato vertical [​](https://docs.plataforma.betha.cloud/docs/design/componentes/checkbox/\#formato-vertical "Direct link to Formato vertical")

- Exemplo
- Vanilla
- React
- Vue

Opção 1

Opção 2

Opção 3

```html
<div class="form-check">
    <input class="form-check-input" type="checkbox" id="chbxv1" value="1">
    <label class="form-check-label" for="chbxv1">Opção 1</label>
</div>
<div class="form-check">
    <input class="form-check-input" type="checkbox" id="chbxv2" value="2">
    <label class="form-check-label" for="chbxv2">Opção 2</label>
</div>
<div class="form-check">
    <input class="form-check-input" type="checkbox" id="chbxv3" value="3" disabled>
    <label class="form-check-label" for="chbxv3">Opção 3</label>
</div>
```

```html
<Form>
    <Form.Group>
        <Form.Check type="checkbox" label="Opção 1" id="chbxv1" />
        <Form.Check type="checkbox" label="Opção 2" id="chbxv2" />
        <Form.Check type="checkbox" label="Opção 3" id="chbxv3" disabled />
    </Form.Group>
</Form>
```

```html
<b-form-group>
    <b-form-checkbox-group v-model="selected" :options="options" name="chbxv" stacked></b-form-checkbox-group>
</b-form-group>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/checkbox/#como-utilizar)
  - [Formato horizontal](https://docs.plataforma.betha.cloud/docs/design/componentes/checkbox/#formato-horizontal)
  - [Formato vertical](https://docs.plataforma.betha.cloud/docs/design/componentes/checkbox/#formato-vertical)