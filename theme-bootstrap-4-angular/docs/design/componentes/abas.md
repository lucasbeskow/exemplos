[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/abas/#docusaurus_skipToContent_fallback)

On this page

As abas são usadas para dividir e organizar o conteúdo, agrupando informações semelhantes na mesma página. Esse componente permite que o usuário visualize o conteúdo sem a necessidade de mudar de página.

As abas podem ser aplicadas de forma horizontal ou vertical, mantendo o mesmo padrão visual.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/abas/\#como-utilizar "Direct link to Como utilizar")

Usa-se sempre que for necessário dividir um conteúdo em seções separadas. As abas não são utilizadas para dividir etapas de um processo. Para fluxos de trabalho utiliza-se o componente [Wizard](https://docs.plataforma.betha.cloud/docs/design/componentes/wizard).

Existem duas variações de abas: horizontais, que aparecem acima do conteúdo, e verticais, que são posicionadas ao lado esquerdo do conteúdo. A utilização de ambas dependerá do layout do ambiente e de como o conteúdo será disposto. As horizontais são mais indicadas quando há menos divisões de conteúdo a serem apresentadas, e as verticais quando houver muitas divisões.

A lagura de cada aba dependerá da nomenclatura utilizada na mesma, por isso recomenda-se o uso de termos curtos, que sejam facilmente reconhecidos pelo usuário e que não prejudiquem a responsividade da página.

### Abas horizontais [​](https://docs.plataforma.betha.cloud/docs/design/componentes/abas/\#abas-horizontais "Direct link to Abas horizontais")

Recomenda-se que todas as abas fiquem sempre visíveis na tela.

- Exemplo
- Vanilla
- Angular
- React
- Vue

Lorem ipsum

Dolor sit amet

```html
<ul class="nav nav-tabs">
  <li class="nav-item">
    <a class="nav-link active" href="#">Aba 1</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Aba 2</a>
  </li>
  <li class="nav-item">
    <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Aba desabilitada</a>
  </li>
</ul>
```

```html
<ul ngbNav #abaHorizontal="ngbNav" [(activeId)]="activeH" class="nav-tabs">
  <li [ngbNavItem]="1">
    <a ngbNavLink>Aba 1</a>
    <ng-template ngbNavContent>
      <p>Lorem ipsum</p>
    </ng-template>
  </li>
  <li [ngbNavItem]="2">
    <a ngbNavLink>Aba 2</a>
    <ng-template ngbNavContent>
      <p>Dolor sit amet</p>
    </ng-template>
  </li>
  <li [ngbNavItem]="3" disabled="true">
    <a ngbNavLink>Aba desabilitada</a>
    <ng-template ngbNavContent>
    </ng-template>
  </li>
</ul>
<div [ngbNavOutlet]="abaHorizontal" class="mt-2"></div>
```

```html
<Tabs defaultActiveKey="aba1">
  <Tab eventKey="aba1" title="Aba 1">
    Lorem ipsum
  </Tab>
  <Tab eventKey="aba2" title="Aba 2">
    Dolor sit amet
  </Tab>
  <Tab eventKey="abaDesabilitada" title="Aba desabilitada" disabled>
  </Tab>
</Tabs>
```

```html
<b-tabs>
    <b-tab title="Aba 1" active>
        <p>Lorem ipsum</p>
    </b-tab>
    <b-tab title="Aba 2">
        <p>Dolor sit amet</p>
    </b-tab>
    <b-tab title="Aba desabilitada" disabled>
        <p></p>
    </b-tab>
</b-tabs>
```

### Abas verticais [​](https://docs.plataforma.betha.cloud/docs/design/componentes/abas/\#abas-verticais "Direct link to Abas verticais")

- Exemplo
- Vanilla
- Angular
- React
- Vue

Lorem ipsum

Dolor sit amet

```html
<div class="d-flex">
  <ul class="nav nav-tabs flex-column">
    <li class="nav-item">
      <a class="nav-link active" href="#">Aba 1</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="#">Aba 2</a>
    </li>
    <li class="nav-item">
      <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Aba desabilitada</a>
    </li>
  </ul>
</div>
```

```html
<div class="d-flex">
  <ul ngbNav #abaVertical="ngbNav" [(activeId)]="activeV" class="nav-tabs" orientation="vertical">
    <li [ngbNavItem]="1">
      <a ngbNavLink>Aba 1</a>
      <ng-template ngbNavContent>
        <p>Lorem ipsum</p>
      </ng-template>
    </li>
    <li [ngbNavItem]="2">
      <a ngbNavLink>Aba 2</a>
      <ng-template ngbNavContent>
        <p>Dolor sit amet</p>
      </ng-template>
    </li>
    <li [ngbNavItem]="3" disabled="true">
      <a ngbNavLink>Aba desabilitada</a>
      <ng-template ngbNavContent>
      </ng-template>
    </li>
  </ul>
  <div [ngbNavOutlet]="abaVertical" class="mt-2"></div>
</div>
```

```html
<Tabs defaultActiveKey="aba1" className="flex-column">
  <Tab eventKey="aba1" title="Aba 1">
    Lorem ipsum
  </Tab>
  <Tab eventKey="aba2" title="Aba 2">
    Dolor sit amet
  </Tab>
  <Tab eventKey="abaDesabilitada" title="Aba desabilitada" disabled>
  </Tab>
</Tabs>
```

```html
<b-tabs vertical>
    <b-tab title="Aba 1" active>
        <p>Lorem ipsum</p>
    </b-tab>
    <b-tab title="Aba 2">
        <p>Dolor sit amet</p>
    </b-tab>
    <b-tab title="Aba desabilitada" disabled>
        <p></p>
    </b-tab>
</b-tabs>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/abas/#como-utilizar)
  - [Abas horizontais](https://docs.plataforma.betha.cloud/docs/design/componentes/abas/#abas-horizontais)
  - [Abas verticais](https://docs.plataforma.betha.cloud/docs/design/componentes/abas/#abas-verticais)