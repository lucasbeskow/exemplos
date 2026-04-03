[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#docusaurus_skipToContent_fallback)

On this page

Este componente é utilizado para organizar dados de forma tabular, permitindo ao usuário localizar uma informação de maneira mais fluída. Também possibilita a edição inline, simulando a experiência de uso de uma planilha.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/\#como-utilizar "Direct link to Como utilizar")

Sempre que houver a necessidade de demonstrar dados em formato de lista.

### Estrutura da listagem [​](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/\#estrutura-da-listagem "Direct link to Estrutura da listagem")

A seguir, são apresentados os elementos principais de uma listagem. Para os casos em que o registro representado pela linha da tabela puder ser visualizado ou editado pelo usuário, utiliza-se a informação principal como link de acesso a esse conteúdo. Outras ações podem listadas em um [dropdown](https://docs.plataforma.betha.cloud/docs/design/componentes/dropdown) na última coluna da lista, conforme demonstrado abaixo:

- Exemplo
- Vanilla
- React

|  | [Coluna 1](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#) | [Coluna 2](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#) | [Coluna 3](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#) | [Coluna 4](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#) |  |
| --- | --- | --- | --- | --- | --- |
|  | ![Avatar](https://picsum.photos/id/237/200)<br>[Informação principal](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/)<br>Informação complementar | Lorem ipsum | [Informação principal](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/)<br>Informação complementar | Dolor sit amet |  |

```html
 <table class="table table-bordered table-fixed">
    <thead>
        <tr>
            <th width="30">
                <div class="form-check">
                    <input type="checkbox" class="form-check-input" id="checkTableAll" />
                    <label class="form-check-label" htmlFor="checkTableAll"></label>
                </div>
            </th>
            <th>
                <a href="#">Coluna 1</a>
            </th>
            <th>
                <a href="#">Coluna 2</a>
            </th>
            <th>
                <a href="#">Coluna 3</a>
            </th>
            <th>
                <a href="#">Coluna 4</a>
            </th>
            <th width="53">
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <div class="form-check">
                    <input type="checkbox" class="form-check-input" id="checkTable1" />
                    <label class="form-check-label" htmlFor="checkTable1"></label>
                </div>
            </td>
            <td>
                <div class="media align-items-center">
                    <img class="rounded-circle size-2 object-cover mr-2" src="https://picsum.photos/id/237/200" alt="Avatar"/>
                    <div class="media-body text-truncate">
                        <p class="m-0 text-truncate"><a href="">Informação principal</a></p>
                        <p class="small m-0 text-muted text-truncate">Informação complementar</p>
                    </div>
                </div>
            </td>
            <td>Lorem ipsum
            </td>
            <td class="text-truncate">
                <p class="m-0 text-truncate"><a href="">Informação principal</a></p>
                <p class="small m-0 text-muted text-truncate">Informação complementar</p>
            </td>
            <td>
                Dolor sit amet
            </td>
            <td>
                <button class="btn btn-link">
                    <i class="mdi mdi-dots-vertical"></i>
                </button>
            </td>
        </tr>
    </tbody>
</table>
```

```html
 <table className="table table-bordered table-fixed">
    <thead>
        <tr>
            <th width="30">
                <div className="form-check">
                    <input type="checkbox" className="form-check-input" id="checkTableAll" />
                    <label className="form-check-label" htmlFor="checkTableAll"></label>
                </div>
            </th>
            <th>
                <a href="#">Coluna 1</a>
            </th>
            <th>
                <a href="#">Coluna 2</a>
            </th>
            <th>
                <a href="#">Coluna 3</a>
            </th>
            <th>
                <a href="#">Coluna 4</a>
            </th>
            <th width="53">
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <div className="form-check">
                    <input type="checkbox" className="form-check-input" id="checkTable1" />
                    <label className="form-check-label" htmlFor="checkTable1"></label>
                </div>
            </td>
            <td>
                <div className="media align-items-center">
                    <img class="rounded-circle size-2 object-cover mr-2" src="https://picsum.photos/id/237/200" alt="Avatar"/>
                    <div class="media-body text-truncate">
                        <p class="m-0 text-truncate"><a href="">Informação principal</a></p>
                        <p class="small m-0 text-muted text-truncate">Informação complementar</p>
                    </div>
                </div>
            </td>
            <td>Lorem ipsum
            </td>
            <td class="text-truncate">
                <p class="m-0 text-truncate"><a href="">Informação principal</a></p>
                <p class="small m-0 text-muted text-truncate">Informação complementar</p>
            </td>
            <td>
                Dolor sit amet
            </td>
            <td>
                <button class="btn btn-link">
                    <i className="mdi mdi-dots-vertical"></i>
                </button>
            </td>
        </tr>
    </tbody>
</table>
```

### Ações inline [​](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/\#a%C3%A7%C3%B5es-inline "Direct link to Ações inline")

- Exemplo
- Vanilla
- React

| [Texto Simples](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#) | [Obrigatório](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#) | Desabilitado | Botões auxiliares | Coluna Textarea |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |

```html
<table class="table table-fixed">
    <thead>
        <tr>
            <th>
                <a href="#">Texto Simples</a>
            </th>
            <th>
                <a href="#" class="required">
                    Obrigatório
                </a>
            </th>
            <th>
                <span>Desabilitado</span>
            </th>
            <th>
                <span>
                    Botões auxiliares
                </span>
            </th>
            <th>
                <span>
                    Coluna Textarea
                </span>
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <input type="text" class="form-control" />
            </td>
            <td>
                <input type="text" class="form-control" />
            </td>
            <td>
                <input type="text" class="form-control" disabled />
            </td>
            <td>
                <div class="input-group">
                    <input type="text" class="form-control"/>
                    <div class="input-group-append">
                        <a class="btn btn-secondary" href="#">
                            <i class="mdi mdi-format-list-checkbox"></i>
                        </a>
                    </div>
                </div>
            </td>
            <td>
                <textarea class="form-control" rows="1"></textarea>
            </td>
        </tr>
    </tbody>
</table>
```

```html
<table className="table table-bordered table-fixed">
    <thead>
        <tr>
            <th>
                <a href="#">Texto Simples</a>
            </th>
            <th>
                <a href="#" className="required">
                    Obrigatório
                </a>
            </th>
            <th>
                <span>Desabilitado</span>
            </th>
            <th>
                <span>
                    Botões auxiliares
                </span>
            </th>
            <th>
                <span>
                    Coluna Textarea
                </span>
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <input type="text" className="form-control" />
            </td>
            <td>
                <input type="text" className="form-control" />
            </td>
            <td>
                <input type="text" className="form-control" disabled />
            </td>
            <td>
                <div className="input-group">
                    <input type="text" className="form-control"/>
                    <div className="input-group-append">
                        <a className="btn btn-secondary" href="#">
                            <i className="mdi mdi-format-list-checkbox"></i>
                        </a>
                    </div>
                </div>
            </td>
            <td>
                <textarea className="form-control" rows="1"></textarea>
            </td>
        </tr>
    </tbody>
</table>
```

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#como-utilizar)
  - [Estrutura da listagem](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#estrutura-da-listagem)
  - [Ações inline](https://docs.plataforma.betha.cloud/docs/design/componentes/listagem/#a%C3%A7%C3%B5es-inline)