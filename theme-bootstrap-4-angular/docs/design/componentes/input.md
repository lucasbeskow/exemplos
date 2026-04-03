[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#docusaurus_skipToContent_fallback)

On this page

Este componente permite o preenchimento de conteúdo alfanumérico.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/input/\#como-utilizar "Direct link to Como utilizar")

Inputs são utilizados em formulários, caixas de diálogo ou em outras situações em que seja necessário permitir que o usuário preencha algum tipo de informação alfanumérica.

### Estrutura básica [​](https://docs.plataforma.betha.cloud/docs/design/componentes/input/\#estrutura-b%C3%A1sica "Direct link to Estrutura básica")

Por padrão, todo input deve possuir um label (rótulo) informando o que deve ser preenchido nele. Quando o input está em foco, sua aparência é alterada, fazendo com que o usuário perceba que campo do formulário está recebendo informação naquele momento.

- Exemplo
- Vanilla
- React
- Vue

Rótulo

```html
<div class="form-group">
    <label for="input1">Rótulo</label>
    <input type="text" class="form-control" id="input1" />
</div>
```

```html
<template>
  <div>
    <b-form-group
      label="Rótulo"
      label-for="input1"
    >
      <b-form-input id="input1" v-model="name"></b-form-input>
    </b-form-group>
  </div>
</template>
```

```html
<Form.Group controlId="inpu1">
    <Form.Label>Rótulo</Form.Label>
    <Form.Control type="text" />
</Form.Group>
```

### Preenchimento obrigatório [​](https://docs.plataforma.betha.cloud/docs/design/componentes/input/\#preenchimento-obrigat%C3%B3rio "Direct link to Preenchimento obrigatório")

Os inputs que recebem informações de preenchimento obrigatório são demonstrados com um asterísco vermelho em seu rótulo, e a mensagem "Este campo é obrigatório" é exibida quando o usuário passa o mouse sobre esse rótulo.

- Exemplo
- Vanilla
- React
- Vue

Rótulo

```html
<div class="form-group">
    <label for="input1" class="required">Rótulo</label>
    <input type="text" class="form-control" id="input1" />
</div>
```

```html
<template>
  <div>
    <b-form-group
      label="Rótulo"
      label-class="required"
      label-for="input1"
    >
      <b-form-input id="input1" v-model="name"></b-form-input>
    </b-form-group>
  </div>
</template>
```

```html
<Form.Group controlId="inpu1">
    <Form.Label class="required">Rótulo</Form.Label>
    <Form.Control type="text" />
</Form.Group>
```

### Placeholder e texto de ajuda [​](https://docs.plataforma.betha.cloud/docs/design/componentes/input/\#placeholder-e-texto-de-ajuda "Direct link to Placeholder e texto de ajuda")

Para casos em que possa não ser claro para o usuário que tipo de informação o input deve receber, podem ser utilizadas duas alternativas: **placeholder** ou **texto de ajuda**.

- Exemplo
- Vanilla
- React

Rótulo

```html
<div class="form-group">
    <label for="input1">Rótulo <i class="mdi mdi-help-circle ml-1" title="Texto de ajuda"></i></label>
    <input type="text" class="form-control" id="input1" placeholder="Texto do placeholder" />
</div>
```

```html
<Form.Group controlId="inpu1">
    <Form.Label>Rótulo <i class="mdi mdi-help-circle ml-1" title="Texto de ajuda"></i></Form.Label>
    <Form.Control type="text" />
</Form.Group>
```

### Addon [​](https://docs.plataforma.betha.cloud/docs/design/componentes/input/\#addon "Direct link to Addon")

Outro recurso utilizado para facilitar o entendimento do tipo de informação que um input deve receber é o **addon**, que pode ser posicionado à esquerda ou à direita do campo. Esse componente também pode receber um botão em vez do texto, para os casos em que haja uma ação relacionada ao preenchimento do input como a abertura de um calendário, por exemplo.

- Exemplo
- Vanilla
- React
- Vue

Rótulo

R$

Rótulo

```html
<!-- Texto - Posicionado à esquerda -->
<div class="form-group">
    <label for="input1">Rótulo</label>
    <div class="input-group">
        <div class="input-group-prepend">
            <span class="input-group-text">R$</span>
        </div>
        <input type="text" class="form-control" id="input1" />
    </div>
</div>

<!-- Texto - Posicionado à direita -->
<div class="form-group">
    <label htmlFor="input1">Rótulo</label>
    <div class="input-group">
        <input type="text" class="form-control" id="input1" />
        <div class="input-group-append">
            <span class="input-group-text">R$</span>
        </div>
    </div>
</div>

<!-- Botão - Posicionado à esquerda -->
<div class="form-group">
    <label for="input1">Rótulo</label>
    <div class="input-group">
        <div class="input-group-prepend">
            <button class="btn btn-secondary" type="button" id="button-addon2">
                <i class="mdi mdi-dots-vertical"></i>
            </button>
        </div>
        <input type="text" class="form-control" id="input1" />
    </div>
</div>

<!-- Botão - Posicionado à direita -->
<div class="form-group">
    <label htmlFor="input1">Rótulo</label>
    <div class="input-group">
        <input type="text" class="form-control" id="input1" />
        <div class="input-group-append">
            <button class="btn btn-secondary" type="button" id="button-addon2">
                <i class="mdi mdi-dots-vertical"></i>
            </button>
        </div>
    </div>
</div>
```

```html
<!-- Texto - Posicionado à esquerda -->
<b-input-group prepend="R$">
    <b-form-input></b-form-input>
</b-input-group>

<!-- Texto - Posicionado à direita -->

<b-input-group append="R$">
    <b-form-input></b-form-input>
</b-input-group>

<!-- Botão - Posicionado à esquerda -->

<b-input-group>
    <b-input-group-prepend>
      <b-button variant="secondary"><i class="mdi mdi-dots-vertical"></i></b-button>
    </b-input-group-prepend>
    <b-form-input type="text"></b-form-input>
</b-input-group>

<!-- Botão - Posicionado à direita -->
<b-input-group>
    <b-form-input type="text"></b-form-input>
    <b-input-group-append>
        <b-button variant="secondary"><i class="mdi mdi-dots-vertical"></i></b-button>
    </b-input-group-append>
</b-input-group>
```

```html
<!-- Texto - Posicionado à esquerda -->
<Form.Group controlId="input1">
    <Form.Label>Rótulo</Form.Label>
    <InputGroup>
        <InputGroup.Prepend>
        <InputGroup.Text id="basic-addon1">R$</InputGroup.Text>
        </InputGroup.Prepend>
        <FormControl/>
  </InputGroup>
</Form.Group>

<!-- Texto - Posicionado à direita -->

<Form.Group controlId="input1">
    <Form.Label>Rótulo</Form.Label>
    <InputGroup>
        <FormControl/>
        <InputGroup.Append>
        <InputGroup.Text>R$</InputGroup.Text>
        </InputGroup.Append>
  </InputGroup>
</Form.Group>

<!-- Botão - Posicionado à esquerda -->
<Form.Group controlId="input1">
    <Form.Label>Rótulo</Form.Label>
    <InputGroup>
        <InputGroup.Prepend>
        <Button variant="secondary"><i class="mdi mdi-dots-vertical"></i></Button>
        </InputGroup.Prepend>
        <FormControl/>
    </InputGroup>
</Form.Group>

<!-- Botão - Posicionado à direita -->
<Form.Group controlId="input1">
    <Form.Label>Rótulo</Form.Label>
    <InputGroup>
        <FormControl/>
        <InputGroup.Append>
        <Button variant="secondary"><i class="mdi mdi-dots-vertical"></i></Button>
        </InputGroup.Append>
    </InputGroup>
</Form.Group>
```

### Informação inconsistente [​](https://docs.plataforma.betha.cloud/docs/design/componentes/input/\#informa%C3%A7%C3%A3o-inconsistente "Direct link to Informação inconsistente")

Quando a informação preenchida no input estiver inconsistente, deve-se utilizar a classe `is-invalid` conforme exemplo a seguir:

- Exemplo
- Vanilla
- React
- Vue

Rótulo

```html
<div class="form-group">
    <label for="input1">Rótulo</label>
    <input type="text" class="form-control is-invalid" id="input1" required />
</div>
```

```html
<template>
  <div>
    <b-form-group
      label="Rótulo"
      label-for="input-1"
      :invalid-feedback="invalidFeedback"
      :state="state"
    >
      <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
    </b-form-group>
  </div>
</template>

<script>
  export default {
    computed: {
      state() {
        return this.name.length >= 4
      },
      invalidFeedback() {
        if (this.name.length > 0) {
          return 'Digite no mínimo 4 caracteres.'
        }
        return 'Por favor, digite algo.'
      }
    },
    data() {
      return {
        name: ''
      }
    }
  }
</script>
```

```html
<InputGroup hasValidation>
  <Form.Control type="text" required isInvalid />
</InputGroup>
```

### Texto longo [​](https://docs.plataforma.betha.cloud/docs/design/componentes/input/\#texto-longo "Direct link to Texto longo")

Para os casos em que houver a necessidade de receber do usuário uma quantidade de caracteres maior do que a que caberia em um input, deve-se utilizar o componente **textarea**:

- Exemplo
- Vanilla
- React
- Vue

Rótulo

```html
<div class="form-group">
    <label for="textarea1">Rótulo</label>
    <textarea class="form-control" id="textarea1" rows="3"></textarea>
</div>
```

```html
 <b-form-textarea id="textarea" v-model="text" rows="3"></b-form-textarea>
```

```html
<Form.Group controlId="input1">
    <Form.Label>Rótulo</Form.Label>
    <Form.Control as="textarea" rows={3} />
</Form.Group>
```

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#como-utilizar)
  - [Estrutura básica](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#estrutura-b%C3%A1sica)
  - [Preenchimento obrigatório](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#preenchimento-obrigat%C3%B3rio)
  - [Placeholder e texto de ajuda](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#placeholder-e-texto-de-ajuda)
  - [Addon](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#addon)
  - [Informação inconsistente](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#informa%C3%A7%C3%A3o-inconsistente)
  - [Texto longo](https://docs.plataforma.betha.cloud/docs/design/componentes/input/#texto-longo)