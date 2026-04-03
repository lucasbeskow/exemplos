[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#docusaurus_skipToContent_fallback)

On this page

## Fixadores [​](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/\#fixadores "Direct link to Fixadores")

Fixadores são classes que ajudam a posicionar elementos fixos `.position-fixed` ou coláveis `.position-sticky` em um dos cantos da tela.
No caso dos elementos fixos, muitas vezes, precisa-se adicionar mais de um fixador para o elemento ficar na posição correta.

- `.top-0` Acima
- `.right-0` Direita
- `.bottom-0` Abaixo
- `.left-0` Esquerda

### Exemplos [​](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/\#exemplos "Direct link to Exemplos")

- Vanilla

```html
<div class="position-relative">
    <div class="position-sticky top-0 zindex-2">
    ...
    </div>
</div>
```

```html
<div class="position-fixed w-100 top-0 left-0 zindex-3">
...
</div>
```

## Z-index [​](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/\#z-index "Direct link to Z-index")

O framework utiliza camadas de posicionamento de elementos através de z-indexes, para que um fique sobre o outro. Você pode utilizar essas classes para posicionar o elemento corretamente na página:

- `.zindex-n1` Elemento oculto
- `.zindex-0` Padrão
- `.zindex-1` Dropdown
- `.zindex-2` **Sticky** (colável)
- `.zindex-3` **Fixed** (fixo)
- `.zindex-4` Modal backdrop
- `.zindex-5` Modal
- `.zindex-6` Popover
- `.zindex-7` Tooltip

## Tamanhos [​](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/\#tamanhos "Direct link to Tamanhos")

Você pode usar as classes de tamanho (altura e largura) para avatares, ou quaisquer elementos que necessitarem.
Os tamanhos disponíveis são:

- `.size-1` 1.75rem²
- `.size-2` 2.25rem²
- `.size-3` 3.25rem²
- `.size-4` 5rem²
- `.size-5` 7.5rem²

### Exemplos [​](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/\#exemplos-1 "Direct link to Exemplos")

![Avatar](https://picsum.photos/id/239/200)![Avatar](https://picsum.photos/id/238/200)![Avatar](https://picsum.photos/id/233/200)![Avatar](https://picsum.photos/id/234/200)![Avatar](https://picsum.photos/id/235/200)

Saiba mais sobre o componente de [Avatar](https://docs.plataforma.betha.cloud/docs/design/componentes/avatar).

## Ajuste de imagem [​](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/\#ajuste-de-imagem "Direct link to Ajuste de imagem")

Você pode fazer uma imagem se ajustar automaticamente e preencher regularmente seu tamanho, utilizando a classe `.object-cover`.

![Avatar](https://www.robin-noorda.com/uploads/1/6/8/3/16830688/3347022_orig.jpg)

Com `.object-cover`

![Avatar](https://www.robin-noorda.com/uploads/1/6/8/3/16830688/3347022_orig.jpg)

Sem a classe

### Exemplo [​](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/\#exemplo "Direct link to Exemplo")

- Vanilla

```html
<img class="object-cover size-5" src="foto.jpg" alt="Imagem"/>
```

- [Fixadores](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#fixadores)
  - [Exemplos](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#exemplos)
- [Z-index](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#z-index)
- [Tamanhos](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#tamanhos)
  - [Exemplos](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#exemplos-1)
- [Ajuste de imagem](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#ajuste-de-imagem)
  - [Exemplo](https://docs.plataforma.betha.cloud/docs/design/layout/helpers/#exemplo)