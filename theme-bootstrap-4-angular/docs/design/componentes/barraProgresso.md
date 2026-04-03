[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/barraProgresso/#docusaurus_skipToContent_fallback)

On this page

Este componente tem o objetivo de apresentar ao usuário o andamento de um processo.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/barraProgresso/\#como-utilizar "Direct link to Como utilizar")

Sempre que o usuário necessite saber o andamento de uma determinada operação, por exemplo, o progresso de um download.

- Exemplo
- Vanilla
- Angular
- React
- Vue

```html
<div class="progress">
  <div class="progress-bar" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
</div>
<div class="progress">
  <div class="progress-bar bg-info" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
</div>
<div class="progress">
  <div class="progress-bar bg-success" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
</div>
<div class="progress">
  <div class="progress-bar bg-warning" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
</div>
<div class="progress">
  <div class="progress-bar bg-danger" role="progressbar" style="width: 80%" aria-valuenow="80" aria-valuemin="0" aria-valuemax="100"></div>
</div>
```

```html
<ngb-progressbar [value]="80"></ngb-progressbar>
<ngb-progressbar type="info" [value]="80"></ngb-progressbar>
<ngb-progressbar type="success" [value]="80"></ngb-progressbar>
<ngb-progressbar type="warning" [value]="80"></ngb-progressbar>
<ngb-progressbar type="danger" [value]="80"></ngb-progressbar>
```

```html
<ProgressBar now={80} />
<ProgressBar variant="info" now={80} />
<ProgressBar variant="success" now={80} />
<ProgressBar variant="warning" now={80} />
<ProgressBar variant="danger" now={80} />
```

```html
<b-progress :value="80" :max="100" show-progress></b-progress>
<b-progress variant="info" :value="80" :max="100" show-progress></b-progress>
<b-progress variant="success" :value="80" :max="100" show-progress></b-progress>
<b-progress variant="warning" :value="80" :max="100" show-progress></b-progress>
<b-progress variant="danger" :value="80" :max="100" show-progress></b-progress>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/barraProgresso/#como-utilizar)