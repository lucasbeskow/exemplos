[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/timeline/#docusaurus_skipToContent_fallback)

On this page

Este componente divide eventos em uma linha do tempo.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/timeline/\#como-utilizar "Direct link to Como utilizar")

Usa-se sempre que for necessário demonstrar eventos que fazem parte de uma mesma linha de tempo, como um histórico, por exemplo.

- Exemplo
- Vanilla
- React

- Fevereiro/2021
- Seg, 16/02

- 10:30:42

[Link para o histórico](https://docs.plataforma.betha.cloud/docs/design/componentes/timeline/)

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.

- 09:15:21

Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.


```html
<div class="d-flex">
    <ul class="nav nav-tabs nav-timeline flex-column">
        <li>
            <span class="badge">Fevereiro/2021</span>
        </li>
        <li>
            <div>
            <p>Seg, 16/02</p>
            </div>
        </li>
        <li>
            <div>
            <small>10:30:42</small>
            </div>
            <p>
            <a href="">Link para o histórico</a><br/>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
            dolore magna aliqua.
            </p>
        </li>
        <li>
            <div>
            <small>09:15:21</small>
            </div>
            <p>
            Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex
            ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat
            nulla pariatur.
            </p>
        </li>
    </ul>
</div>
```

```html
<div className="d-flex my-5">
  <ul className="nav nav-tabs nav-timeline flex-column">
    <li>
      <span className="badge">Fevereiro/2021</span>
    </li>
    <li>
      <div>
        <p>Seg, 16/02</p>
      </div>
    </li>
    <li>
      <div>
        <small>10:30:42</small>
      </div>
      <p>
        <a href="">Link para o histórico</a><br/>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
        dolore magna aliqua.
      </p>
    </li>
    <li>
      <div>
        <small>09:15:21</small>
      </div>
      <p>
        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex
        ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat
        nulla pariatur.
      </p>
    </li>
  </ul>
</div>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/timeline/#como-utilizar)