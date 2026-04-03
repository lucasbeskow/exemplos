[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/alerta/#docusaurus_skipToContent_fallback)

On this page

Este componente tem como objetivo mostrar ao usuário alguma informação importante do sistema.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/alerta/\#como-utilizar "Direct link to Como utilizar")

Sempre que for necessário mostrar informações importantes do sistema, sem que seja necessário interromper o fluxo de trabalho do usuário, e sim apenas chamar sua atenção para informações específicas. Os ícones sempre devem antecipar a mensagem a ser apresentada.

Este componente deve sempre ser apresentado na parte superior do ambiente ou dentro de componentes como popover, modal, cards, entre outros, ocupando toda a largura disponível. Existem quatro estados possíveis para os avisos: `info`, `success`, `warning` e `danger`.

### Personalizado [​](https://docs.plataforma.betha.cloud/docs/design/componentes/alerta/\#personalizado "Direct link to Personalizado")

- Exemplo
- Vanilla
- Angular
- React
- Vue

Info: indica uma mudança ou ação informativa neutra.

```html
<div class="alert alert-info" role="alert">
  <div class="form-row align-items-center">
    <div class="col-auto">
      <i class="h5 mdi mdi-star mb-0"></i>
    </div>
    <div class="col">Info: indica uma mudança ou ação informativa neutra.</div>
  </div>
</div>
```

```html
<ngb-alert [type]="'info'">
  <div class="form-row align-items-center">
    <div class="col-auto">
      <i class="h5 mdi mdi-star mb-0"></i>
    </div>
    <div class="col">Info: indica uma mudança ou ação informativa neutra.</div>
  </div>
</ngb-alert>
```

```html
<Alert variant="info">
  <div class="form-row align-items-center">
    <div class="col-auto">
      <i class="h5 mdi mdi-star mb-0"></i>
    </div>
    <div class="col">Info: indica uma mudança ou ação informativa neutra.</div>
  </div>
</Alert>
```

```html
<b-alert variant="info">
  <div class="form-row align-items-center">
    <div class="col-auto">
      <i class="h5 mdi mdi-star mb-0"></i>
    </div>
    <div class="col">Info: indica uma mudança ou ação informativa neutra.</div>
  </div>
</b-alert>
```

### Padrões [​](https://docs.plataforma.betha.cloud/docs/design/componentes/alerta/\#padr%C3%B5es "Direct link to Padrões")

Os padrões de alerta com ícone pode ser utilizada aplicando-se a classe `alert-icon`. Observe abaixo em que ocasião cada tipo deve ser utilizado:

- Exemplo
- Vanilla
- Angular
- React
- Vue

Info: indica uma mudança ou ação informativa neutra.

Success: indica uma ação bem sucedida ou positiva.

Warning: indica algo que requer a atenção do usuário.

Danger: indica uma ação crítica ou informa inconsistências.

```html
<div class="alert alert-icon alert-info" role="alert">
  Mensagem do alerta.
</div>
<div class="alert alert-icon alert-success" role="alert">
  Mensagem do alerta.
</div>
<div class="alert alert-icon alert-warning" role="alert">
  Mensagem do alerta.
</div>
<div class="alert alert-icon alert-danger" role="alert">
  Mensagem do alerta.
</div>
```

```html
<ngb-alert [type]="'info'" class="alert-icon">Mensagem do alerta.</ngb-alert>
<ngb-alert [type]="'success'" class="alert-icon">Mensagem do alerta.</ngb-alert>
<ngb-alert [type]="'warning'" class="alert-icon">Mensagem do alerta.</ngb-alert>
<ngb-alert [type]="'danger'" class="alert-icon">Mensagem do alerta.</ngb-alert>
```

```html
<Alert variant="info" className="alert-icon">Mensagem do alerta.</Alert>
<Alert variant="success" className="alert-icon">Mensagem do alerta.</Alert>
<Alert variant="warning" className="alert-icon">Mensagem do alerta.</Alert>
<Alert variant="danger" className="alert-icon">Mensagem do alerta.</Alert>
```

```html
<b-alert variant="info" class="alert-icon">Mensagem do alerta.</b-alert>
<b-alert variant="success" class="alert-icon">Mensagem do alerta.</b-alert>
<b-alert variant="warning" class="alert-icon">Mensagem do alerta.</b-alert>
<b-alert variant="danger" class="alert-icon">Mensagem do alerta.</b-alert>
```

* * *

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/alerta/#como-utilizar)
  - [Personalizado](https://docs.plataforma.betha.cloud/docs/design/componentes/alerta/#personalizado)
  - [Padrões](https://docs.plataforma.betha.cloud/docs/design/componentes/alerta/#padr%C3%B5es)