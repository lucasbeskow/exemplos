[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard/#docusaurus_skipToContent_fallback)

On this page

Este componente é utilizado para demonstrar uma rotina que depende da conclusão de etapas para ser finalizada.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard/\#como-utilizar "Direct link to Como utilizar")

Sempre que for necessário dividir em etapas (passo a passo) uma rotina da interface. As etapas já finalizadas pelo usuário são demonstradas com o ícone .

### Formato horizontal [​](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard/\#formato-horizontal "Direct link to Formato horizontal")

- Exemplo
- Vanilla
- Angular
- React
- Vue

Conteúdo da etapa 1

Conteúdo da etapa 2

Conteúdo da etapa 3

```html
<ul class="nav nav-tabs nav-wizard">
    <li class="nav-item">
        <a class="nav-link checked" href="#">Etapa 1</a>
    </li>
    <li class="nav-item">
        <a class="nav-link checked" href="#">Etapa 2</a>
    </li>
    <li class="nav-item">
        <a class="nav-link active" href="#">Etapa 3</a>
    </li>
    <li class="nav-item">
        <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Etapa 4</a>
    </li>
</ul>
```

```html
<ul ngbNav #wizard="ngbNav" [(activeId)]="activeWizardStep" class="nav-tabs nav-wizard">
    <li [ngbNavItem]="1">
    <a ngbNavLink class="checked">Etapa 1</a>
    <ng-template ngbNavContent>
        <p>Conteúdo da etapa 1</p>
    </ng-template>
    </li>
    <li [ngbNavItem]="2">
    <a ngbNavLink class="checked">Etapa 2</a>
    <ng-template ngbNavContent>
        <p>Conteúdo da etapa 2</p>
    </ng-template>
    </li>
    <li [ngbNavItem]="3">
    <a ngbNavLink>Etapa 3</a>
    <ng-template ngbNavContent>
        Conteúdo da etapa 3
    </ng-template>
    </li>
    <li [ngbNavItem]="4" disabled="true">
    <a ngbNavLink>Etapa 4</a>
    <ng-template ngbNavContent>
        Conteúdo da etapa 4
    </ng-template>
    </li>
</ul>
<div [ngbNavOutlet]="wizard" class="mt-2"></div>
```

```html
<ReactTabs defaultActiveKey="etapa3" className="nav-wizard">
    <Tab eventKey="etapa1" title="Etapa 1" tabClassName="checked">
    Conteúdo da etapa 1
    </Tab>
    <Tab eventKey="etapa2" title="Etapa 2" tabClassName="checked">
    Conteúdo da etapa 2
    </Tab>
    <Tab eventKey="etapa3" title="Etapa 3">
    Conteúdo da etapa 3
    </Tab>
    <Tab eventKey="etapa4" title="Etapa 4" disabled>
    </Tab>
</ReactTabs>
```

```html
<b-tabs nav-class="nav-wizard">
    <b-tab title="Etapa 1" title-link-class="checked">
        <p>Conteúdo da etapa 1</p>
    </b-tab>
    <b-tab title="Etapa 2" title-link-class="checked">
        <p>Conteúdo da etapa 2</p>
    </b-tab>
    <b-tab title="Etapa 3" active>
        <p>Conteúdo da etapa 3</p>
    </b-tab>
    <b-tab title="Etapa 4" disabled>
        <p></p>
    </b-tab>
</b-tabs>
```

### Formato vertical [​](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard/\#formato-vertical "Direct link to Formato vertical")

- Exemplo
- Vanilla
- Angular
- React
- Vue

Conteúdo da etapa 1

Conteúdo da etapa 2

Conteúdo da etapa 3

```html
<div class="d-flex">
    <ul class="nav nav-tabs nav-wizard flex-column">
        <li class="nav-item">
            <a class="nav-link checked" href="#">Etapa 1</a>
        </li>
        <li class="nav-item">
            <a class="nav-link checked" href="#">Etapa 2</a>
        </li>
        <li class="nav-item">
            <a class="nav-link active" href="#">Etapa 3</a>
        </li>
        <li class="nav-item">
            <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Etapa 4</a>
        </li>
    </ul>
</div>
```

```html
<div class="d-flex">
    <ul ngbNav #wizardV="ngbNav" [(activeId)]="activeWizardVStep" class="nav-tabs nav-wizard" orientation="vertical">
    <li [ngbNavItem]="1">
        <a ngbNavLink class="checked">Etapa 1</a>
        <ng-template ngbNavContent>
        <p>Conteúdo da etapa 1</p>
        </ng-template>
    </li>
    <li [ngbNavItem]="2">
        <a ngbNavLink class="checked">Etapa 2</a>
        <ng-template ngbNavContent>
        <p>Conteúdo da etapa 2</p>
        </ng-template>
    </li>
    <li [ngbNavItem]="3">
        <a ngbNavLink>Etapa 3</a>
        <ng-template ngbNavContent>
        Conteúdo da etapa 3
        </ng-template>
    </li>
    <li [ngbNavItem]="4" disabled="true">
        <a ngbNavLink>Etapa 4</a>
        <ng-template ngbNavContent>
        Conteúdo da etapa 4
        </ng-template>
    </li>
    </ul>
    <div [ngbNavOutlet]="wizardV" class="mt-2"></div>
</div>
```

```html
<ReactTabs defaultActiveKey="etapa3" className="nav-wizard flex-column">
    <Tab eventKey="etapa1" title="Etapa 1" tabClassName="checked">
    Conteúdo da etapa 1
    </Tab>
    <Tab eventKey="etapa2" title="Etapa 2" tabClassName="checked">
    Conteúdo da etapa 2
    </Tab>
    <Tab eventKey="etapa3" title="Etapa 3">
    Conteúdo da etapa 3
    </Tab>
    <Tab eventKey="etapa4" title="Etapa 4" disabled>
    </Tab>
</ReactTabs>
```

```html
<b-tabs nav-class="nav-wizard" vertical="true">
    <b-tab title="Etapa 1" title-link-class="checked">
        <p>Conteúdo da etapa 1</p>
    </b-tab>
    <b-tab title="Etapa 2" title-link-class="checked">
        <p>Conteúdo da etapa 2</p>
    </b-tab>
    <b-tab title="Etapa 3" active>
        <p>Conteúdo da etapa 3</p>
    </b-tab>
    <b-tab title="Etapa 4" disabled>
        <p></p>
    </b-tab>
</b-tabs>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard/#como-utilizar)
  - [Formato horizontal](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard/#formato-horizontal)
  - [Formato vertical](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard/#formato-vertical)