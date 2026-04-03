[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/radio/#docusaurus_skipToContent_fallback)

On this page

Este componente permite a seleção de uma única opção de um grupo de alternativas.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/radio/\#como-utilizar "Direct link to Como utilizar")

É utilizado em situações em que é permitido ao usuário escolher um único item dentro de um grupo de opções.

### Formato horizontal [​](https://docs.plataforma.betha.cloud/docs/design/componentes/radio/\#formato-horizontal "Direct link to Formato horizontal")

- Exemplo
- Vanilla
- React
- Vue

Opção 1

Opção 2

Opção 3

```html
<div class="form-check form-check-inline">
    <input class="form-check-input" type="radio" id="rdh1" value="1">
    <label class="form-check-label" for="rdh1">Opção 1</label>
</div>
<div class="form-check form-check-inline">
    <input class="form-check-input" type="radio" id="rdh2" value="2">
    <label class="form-check-label" for="rdh2">Opção 2</label>
</div>
<div class="form-check form-check-inline">
    <input class="form-check-input" type="radio" id="rdh3" value="3" disabled>
    <label class="form-check-label" for="rdh3">Opção 3</label>
</div>
```

```html
<Form>
    <Form.Group>
        <Form.Check type="radio" label="Opção 1" inline id="rdh1" />
        <Form.Check type="radio" label="Opção 2" inline id="rdh2" />
        <Form.Check type="radio" label="Opção 3" inline id="rdh3" disabled />
    </Form.Group>
</Form>
```

```html
<b-form-group>
    <b-form-radio v-model="selected" name="rd" value="1">Opção 1</b-form-radio>
    <b-form-radio v-model="selected" name="rd" value="2">Opção 2</b-form-radio>
    <b-form-radio v-model="selected" name="rd" value="3" disabled="true">Opção 3</b-form-radio>
</b-form-group>
```

### Formato vertical [​](https://docs.plataforma.betha.cloud/docs/design/componentes/radio/\#formato-vertical "Direct link to Formato vertical")

- Exemplo
- Vanilla
- React
- Vue

Opção 1

Opção 2

Opção 3

```html
<div class="form-check">
    <input class="form-check-input" type="radio" id="rdv1" value="1">
    <label class="form-check-label" for="rdv1">Opção 1</label>
</div>
<div class="form-check">
    <input class="form-check-input" type="radio" id="rdv2" value="2">
    <label class="form-check-label" for="rdv2">Opção 2</label>
</div>
<div class="form-check">
    <input class="form-check-input" type="radio" id="rdv3" value="3" disabled>
    <label class="form-check-label" for="rdv3">Opção 3</label>
</div>
```

```html
<Form>
    <Form.Group>
        <Form.Check type="radio" label="Opção 1" id="rdv1" />
        <Form.Check type="radio" label="Opção 2" id="rdv2" />
        <Form.Check type="radio" label="Opção 3" id="rdv3" disabled />
    </Form.Group>
</Form>
```

```html
<b-form-group stacked>
    <b-form-radio v-model="selected" name="rd" value="1">Opção 1</b-form-radio>
    <b-form-radio v-model="selected" name="rd" value="2">Opção 2</b-form-radio>
    <b-form-radio v-model="selected" name="rd" value="3" disabled="true">Opção 3</b-form-radio>
</b-form-group>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/radio/#como-utilizar)
  - [Formato horizontal](https://docs.plataforma.betha.cloud/docs/design/componentes/radio/#formato-horizontal)
  - [Formato vertical](https://docs.plataforma.betha.cloud/docs/design/componentes/radio/#formato-vertical)