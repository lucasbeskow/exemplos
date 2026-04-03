[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/switch/#docusaurus_skipToContent_fallback)

On this page

Este componente permite ativar e desativar opções, bem como representar visualmente quais itens estão ativos e inativos.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/switch/\#como-utilizar "Direct link to Como utilizar")

É possível utilizá-lo em elementos isolados, listagens, tabelas, cards, etc. Por padrão, este componente é alinhado verticalmente em formato de lista.

A descrição do switch deve representar algo que possa ser ativado ou desativado, e nunca deve ser alterada para se adaptar à escolha do usuário. Observe o exemplo a seguir:

Receber notificações por e-mail

### Formato horizontal [​](https://docs.plataforma.betha.cloud/docs/design/componentes/switch/\#formato-horizontal "Direct link to Formato horizontal")

- Exemplo
- Vanilla
- React
- Vue

4G

Bluetooth

Wi-Fi

```html
<div class="custom-control custom-switch custom-control-inline">
    <input type="checkbox" class="custom-control-input" id="swth1">
    <label class="custom-control-label" for="swth1">4G</label>
</div>
<div class="custom-control custom-switch custom-control-inline">
    <input type="checkbox" class="custom-control-input" id="swth2">
    <label class="custom-control-label" for="swth2">Bluetooth</label>
</div>
<div class="custom-control custom-switch custom-control-inline">
    <input type="checkbox" class="custom-control-input" id="swth3" disabled>
    <label class="custom-control-label" for="swth3">Wi-Fi</label>
</div>
```

```html
<Form>
    <Form.Group>
        <Form.Check type="switch" label="4G" inline id="swth1" />
        <Form.Check type="switch" label="Bluetooth" inline id="swth2" />
        <Form.Check type="switch" label="Wi-Fi" inline id="swth3" disabled />
    </Form.Group>
</Form>
```

```html
<b-form-group>
    <b-form-checkbox-group v-model="selected" :options="options" name="swth" switch></b-form-checkbox-group>
</b-form-group>
```

### Formato vertical [​](https://docs.plataforma.betha.cloud/docs/design/componentes/switch/\#formato-vertical "Direct link to Formato vertical")

- Exemplo
- Vanilla
- React
- Vue

4G

Bluetooth

Wi-Fi

```html
<div class="custom-control custom-switch">
    <input type="checkbox" class="custom-control-input" id="swtv1">
    <label class="custom-control-label" for="swtv1">4G</label>
</div>
<div class="custom-control custom-switch">
    <input type="checkbox" class="custom-control-input" id="swtv2">
    <label class="custom-control-label" for="swtv2">Bluetooth</label>
</div>
<div class="custom-control custom-switch">
    <input type="checkbox" class="custom-control-input" id="swtv3" disabled>
    <label class="custom-control-label" for="swtv3">Wi-Fi</label>
</div>
```

```html
<Form>
    <Form.Group>
        <Form.Check type="switch" label="Opção 1" id="swtv1" />
        <Form.Check type="switch" label="Opção 2" id="swtv2" />
        <Form.Check type="switch" label="Opção 3" id="swtv3" disabled />
    </Form.Group>
</Form>
```

```html
<b-form-group>
    <b-form-checkbox-group v-model="selected" :options="options" name="swtv" switch stacked></b-form-checkbox-group>
</b-form-group>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/switch/#como-utilizar)
  - [Formato horizontal](https://docs.plataforma.betha.cloud/docs/design/componentes/switch/#formato-horizontal)
  - [Formato vertical](https://docs.plataforma.betha.cloud/docs/design/componentes/switch/#formato-vertical)