[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/#docusaurus_skipToContent_fallback)

On this page

Este componente tem o objetivo de apresentar ao usuário uma ação disponível na interface.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/\#como-utilizar "Direct link to Como utilizar")

Os botões são utilizados para executar ações em primeiro plano (quando ocorre uma mudança imediata na interface) ou em segundo plano (quando visualmente nada muda na interface). Eles podem ser compostos por textos, ícones ou ambos. O texto de dentro dos botões deve ser apresentado em letras maiúsculas.

Existem cores específicas para cada contexto, conforme referência abaixo:

| Estado | Botão | Contexto |
| :-- | --- | --- |
| `primary` | Botão | Ação principal da interface. Deve ser utilizado apenas um botão desse tipo por formulário ou recurso. |
| `secondary` | Botão | Ação secundária. Utilizado sempre que a ação não precisar de um contexto específico. |
| `info` | Botão | Ação de destaque. Utilizado para destacar uma ação que não se encaixe em outros contextos. |
| `success` | Botão | Ação relacionada a sucesso. É o botão padrão para a adição de registros. |
| `warning` | Botão | Ação relacionada a alerta. Utilizado em situações que necessitem da atenção do usuário. |
| `danger` | Botão | Ação crítica. Utilizado em confirmações ou em ações que não podem ser desfeitas ou que requerem muita atenção do usuário. |
| `link` | Botão | Ação secundária sem destaque. Utilizado em casos onde a ação não precisa estar evidente na interface |

### Tamanhos [​](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/\#tamanhos "Direct link to Tamanhos")

Além do padrão, existem outros dois tamanhos possíveis para o botão:

| Tamanho | Botão |
| :-- | --- |
| `sm` | Botão |
| `lg` | Botão |

Por consistência e acessibilidade, deve-se usar o tamanho padrão na maioria dos casos. Salvos espaços muito pequenos que precisem utilizar o tamanho "sm". Já o tamanho "lg" deve ser usado apenas em casos excepcionais.

### Botão adicionar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/\#bot%C3%A3o-adicionar "Direct link to Botão adicionar")

Por padrão, o botão usado para adicionar um registro é apresentado com o ícone de "+" antes do rótulo, e utiliza a variação `success`. A classe `btn-add`, que não existe originalmente no Bootstrap, deve ser utilizada neste caso. Deve-se utilizar também o elemento `aria-label="Adicionar XXX"`, onde "XXX" é o texto do interior do botão.

| Classe | Botão |
| :-- | --- |
| `btn-add` | Documento |

```html
<button class="btn btn-success btn-add" aria-label="Adicionar Documento">Documento</button>
```

### Botões agrupados [​](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/\#bot%C3%B5es-agrupados "Direct link to Botões agrupados")

O grupo de botão é utilizado para representar botões que tenham relação entre si.

- Exemplo
- Vanilla
- React
- Vue

Botão 1Botão 2Botão 3

```html
<div class="btn-group" role="group" aria-label="Grupo de botões">
  <button type="button" class="btn btn-secondary active">Botão 1</button>
  <button type="button" class="btn btn-secondary">Botão 2</button>
  <button type="button" class="btn btn-secondary">Botão 3</button>
</div>
```

```html
<ButtonGroup aria-label="Grupo de botões">
  <Button variant="secondary" size="sm" className="active">Botão 1</Button>
  <Button variant="secondary" size="sm">Botão 2</Button>
  <Button variant="secondary" size="sm">Botão 3</Button>
</ButtonGroup>
```

```html
<b-button-group>
  <b-button variant="secondary">Botão 1</b-button>
  <b-button variant="secondary">Botão 2</b-button>
  <b-button variant="secondary">Botão 3</b-button>
</b-button-group>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/#como-utilizar)
  - [Tamanhos](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/#tamanhos)
  - [Botão adicionar](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/#bot%C3%A3o-adicionar)
  - [Botões agrupados](https://docs.plataforma.betha.cloud/docs/design/componentes/botao/#bot%C3%B5es-agrupados)