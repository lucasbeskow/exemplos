[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/paginacao/#docusaurus_skipToContent_fallback)

On this page

Este componente tem o objetivo de permitir a navegação entre páginas de itens de uma lista e de possibilitar ao usuário escolher a quantidade máxima de registros a ser exibida por página.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/paginacao/\#como-utilizar "Direct link to Como utilizar")

Sempre que houver a necessidade de separar em páginas os itens de uma lista. Deve ser posicionado logo abaixo do último item de cada página, sendo que a barra de navegação deve ser alinhada à direita e o detalhamento de registros à esquerda da lista.

### Barra de navegação [​](https://docs.plataforma.betha.cloud/docs/design/componentes/paginacao/\#barra-de-navega%C3%A7%C3%A3o "Direct link to Barra de navegação")

Esta barra é formada por, no máximo, seis botões: o botão "Anterior"; até quatro botões representando o número das páginas; e o botão "Próxima", nesta ordem. Os botões "Anterior" e "Próxima" ficam desabilitados quando o usuário estiver na primeira ou na última páginas, respectivamente. Se o usuário estiver na página 5, por exemplo, devem ser exibidos os botões "Anterior", "2", "3", "4", "5" e "Próxima".

Nos casos em que houver menos de quatro páginas de resultados, devem ser exibidos, entre os botões "Anterior" e "Próxima", os botões referentes ao número de páginas existentes. Observe abaixo cenários em que as regras mencionadas são aplicadas:

**O usuário está na primeira página:**

**O usuário está na última página:**

**Existem apenas 3 páginas de resultados e o usuário está na segunda:**

- Vanilla
- Angular
- React
- Vue

```html
<nav class="float-right">
    <ul class="pagination">
        <li class="page-item"><a class="page-link" href="#"><i class="mdi mdi-chevron-left mr-1"></i>Anterior</a></li>
        <li class="page-item"><a class="page-link" href="#">1</a></li>
        <li class="page-item active"><a class="page-link" href="#">2</a></li>
        <li class="page-item"><a class="page-link" href="#">3</a></li>
        <li class="page-item"><a class="page-link" href="#">Próxima<i class="mdi mdi-chevron-right ml-1"></i></a></li>
    </ul>
</nav>
```

```html
<ngb-pagination [collectionSize]="70" [(page)]="page">
    <ng-template ngbPaginationPrevious><i class="mdi mdi-chevron-left mr-1"></i>Anterior</ng-template>
    <ng-template ngbPaginationNext>Próxima<i class="mdi mdi-chevron-right ml-1"></i></ng-template>
    <ng-template ngbPaginationNumber let-p>{{ p }}</ng-template>
</ngb-pagination>
```

```html
<Pagination>
    <Pagination.Prev><i class="mdi mdi-chevron-left mr-1"></i>Anterior</Pagination.Prev>
    <Pagination.Item>{1}</Pagination.Item>
    <Pagination.Item>{2}</Pagination.Item>
    <Pagination.Item active>{3}</Pagination.Item>
    <Pagination.Item>{4}</Pagination.Item>
    <Pagination.Next>Próxima<i class="mdi mdi-chevron-right ml-1"></i></Pagination.Next>
</Pagination>
```

```html
<b-pagination v-model="currentPage" :total-rows="rows" :per-page="perPage" class="mt-4" aria-controls="my-table" hide-goto-end-buttons="true">
    <template #prev-text><i class="mdi mdi-chevron-left mr-1"></i>Anterior</template>
    <template #next-text>Próxima<i class="mdi mdi-chevron-right ml-1"></i></template>
</b-pagination>
```

### Detalhamento de registros [​](https://docs.plataforma.betha.cloud/docs/design/componentes/paginacao/\#detalhamento-de-registros "Direct link to Detalhamento de registros")

Nos casos em que se mostrar necessário detalhar o número de registros separados em páginas, deve-se utilizar o padrão demonstrado abaixo.

O detalhamento de registros é dividido em: número do primeiro e do último registros demonstrados na página atual separados por hífen; a palavra "de" seguida do número total de registros que serão exibidos em todas as páginas; um select com as opções 20, 50 e 100, que indicam o número de resultados a serem exibidos por página; e a frase "resultados por página".

1-20 de 100 resultados por página

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/paginacao/#como-utilizar)
  - [Barra de navegação](https://docs.plataforma.betha.cloud/docs/design/componentes/paginacao/#barra-de-navega%C3%A7%C3%A3o)
  - [Detalhamento de registros](https://docs.plataforma.betha.cloud/docs/design/componentes/paginacao/#detalhamento-de-registros)