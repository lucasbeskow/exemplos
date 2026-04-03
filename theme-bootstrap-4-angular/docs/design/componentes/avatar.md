[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/avatar/#docusaurus_skipToContent_fallback)

On this page

Os avatares são imagens utilizadas para identificar os usuários. Eles podem ser únicos ou agrupados.

## Único [​](https://docs.plataforma.betha.cloud/docs/design/componentes/avatar/\#%C3%BAnico "Direct link to Único")

O avatar único pode ser usado em listagens, cards ou em conjunto com qualquer outro elemento que o necessite.

- Exemplo
- Vanilla
- React
- Vue

![Avatar](https://picsum.photos/id/236/200)

```html
<img class="avatar size-2" src="/foto.jpg" />
```

```html
<b-avatar src="/foto.jpg" variant="light" size="2.25rem"></b-avatar>
```

```html
<img className="avatar size-2" src="/foto.jpg" alt="Avatar" />
```

## Agrupados [​](https://docs.plataforma.betha.cloud/docs/design/componentes/avatar/\#agrupados "Direct link to Agrupados")

Avatares agrupados podem ser usados para identificar grupos de usuários rapidamente.

- Exemplo
- Vanilla
- React
- Vue

![Avatar](https://picsum.photos/id/231/200)

![Avatar](https://picsum.photos/id/232/200)

![Avatar](https://picsum.photos/id/233/200)

![Avatar](https://picsum.photos/id/234/200)

![Avatar](https://picsum.photos/id/235/200)

```html
<div class="d-block pr-2">
    <div class="d-inline-block mr-n2">
        <img class="rounded-circle size-2 border" src="/foto.jpg" alt="Avatar"/>
    </div>
    <div class="d-inline-block mr-n2">
        <img class="rounded-circle size-2 border" src="/foto.jpg" alt="Avatar"/>
    </div>
    <div class="d-inline-block mr-n2">
        <img class="rounded-circle size-2 border" src="/foto.jpg" alt="Avatar"/>
    </div>
    <div class="d-inline-block mr-n2">
        <img class="rounded-circle size-2 border" src="/foto.jpg" alt="Avatar"/>
    </div>
    <div class="d-inline-block mr-n2">
        <img class="rounded-circle size-2 border" src="/foto.jpg" alt="Avatar"/>
    </div>
</div>
```

```html
<b-avatar-group size="2.25rem">
  <b-avatar src="/foto.jpg" variant="light"></b-avatar>
  <b-avatar src="/foto.jpg" variant="light"></b-avatar>
  <b-avatar src="/foto.jpg" variant="light"></b-avatar>
  <b-avatar src="/foto.jpg" variant="light"></b-avatar>
  <b-avatar src="/foto.jpg" variant="light"></b-avatar>
</b-avatar-group>
```

```html
<div className="d-block pr-2">
    <div className="d-inline-block mr-n2">
        <img className="rounded-circle size-2 border" src="https://picsum.photos/id/231/200" alt="Avatar"/>
    </div>
    <div className="d-inline-block mr-n2">
        <img className="rounded-circle size-2 border" src="https://picsum.photos/id/232/200" alt="Avatar"/>
    </div>
    <div className="d-inline-block mr-n2">
        <img className="rounded-circle size-2 border" src="https://picsum.photos/id/233/200" alt="Avatar"/>
    </div>
    <div className="d-inline-block mr-n2">
        <img className="rounded-circle size-2 border" src="https://picsum.photos/id/234/200" alt="Avatar"/>
    </div>
    <div className="d-inline-block mr-n2">
        <img className="rounded-circle size-2 border" src="https://picsum.photos/id/235/200" alt="Avatar"/>
    </div>
</div>
```

Veja todos os tamanhos de avatares disponíveis em [Classes extras](https://docs.plataforma.betha.cloud/docs/design/layout/helpers#tamanhos).

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Único](https://docs.plataforma.betha.cloud/docs/design/componentes/avatar/#%C3%BAnico)
- [Agrupados](https://docs.plataforma.betha.cloud/docs/design/componentes/avatar/#agrupados)