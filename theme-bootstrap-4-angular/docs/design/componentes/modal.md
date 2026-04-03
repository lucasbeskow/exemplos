[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/componentes/modal/#docusaurus_skipToContent_fallback)

On this page

Este componente tem como objetivo apresentar uma funcionalidade complementar em um ambiente, de modo que o conteúdo principal apareça em segundo plano enquanto o usuário realiza o procedimento relacionado à janela que foi aberta.

## Como utilizar [​](https://docs.plataforma.betha.cloud/docs/design/componentes/modal/\#como-utilizar "Direct link to Como utilizar")

Sempre que for necessário exibir algo em uma janela que requer a atenção e ação do usuário. Esse componente oferece uma forma de coleta de dados que otimiza o uso do espaço da página, mantendo mensagens e formulários ocultos e os exibindo apenas quando necessário. Existem modelos e tamanhos diferentes, observe os exemplos a seguir.

Por padrão, uma modal é composta por cabeçalho, onde fica o título e o botão fechar, corpo, onde fica o conteúdo, geralmente um formulário, e rodapé, onde são apresentados os botões de ação da modal.

O título da modal vai aqui

×Close

O conteúdo da modal vai aqui.

SalvarCancelar

- Exemplo
- Vanilla
- Angular
- React
- Vue

Abrir modal

```html
<!-- Botão para abrir a modal -->
<button type="button" class="btn btn-secondary" data-toggle="modal" data-target="#modalExemplo">
  Abrir modal
</button>

<!-- Modal -->
<div class="modal fade" id="modalExemplo" tabindex="-1" aria-labelledby="modalExemploLabel" aria-hidden="true">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="modalExemploLabel">Título da modal</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Fechar">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        Conteúdo da modal
      </div>
      <div class="modal-footer">
          <button type="button" class="btn btn-primary mr-1">Salvar</button>
        <button type="button" class="btn btn-secondary" data-dismiss="modal">Cancelar</button>
      </div>
    </div>
  </div>
</div>
```

```html
<ng-template #content let-modal>
  <div class="modal-header">
    <h4 class="modal-title" id="modal-basic-title">Título da modal</h4>
    <button type="button" class="close" aria-label="Close" (click)="modal.dismiss('Cross click')">
      <span aria-hidden="true">&times;</span>
    </button>
  </div>
  <div class="modal-body">
    Conteúdo da modal
  </div>
  <div class="modal-footer">
    <button type="button" class="btn btn-primary" (click)="modal.close('Save click')">Salvar</button>
    <button type="button" class="btn btn-secondary" (click)="modal.close()">Cancelar</button>
  </div>
</ng-template>

<button class="btn btn-secondary" (click)="open(content)">Abrir modal</button>
```

```html
() => {
  const [show, setShow] = useState(false);
  const handleClose = () => setShow(false);
  const handleShow = () => setShow(true);
  return (
    <>
      <Button variant="secondary" size="sm" onClick={handleShow}>
        Abrir modal
      </Button>
      <Modal show={show} onHide={handleClose}>
        <Modal.Header closeButton>
          <Modal.Title>Título da modal</Modal.Title>
        </Modal.Header>
        <Modal.Body>Conteúdo da modal</Modal.Body>
        <Modal.Footer>
        <Button variant="primary" onClick={handleClose}>
            Salvar
          </Button>
          <Button variant="secondary" onClick={handleClose}>
            Cancelar
          </Button>
        </Modal.Footer>
      </Modal>
    </>
  );
}
```

```html
<div>
  <b-button v-b-modal.modal-1>Abrir modal</b-button>
  <b-modal id="modal-1" title="Título da modal">
    Conteúdo da modal
  </b-modal>
</div>
```

O uso da estrutura acima requer a instalação das bibliotecas descritas em [Tema para Bootstrap 4](https://docs.plataforma.betha.cloud/docs/design/implementacoes/bootstrap4).

- [Como utilizar](https://docs.plataforma.betha.cloud/docs/design/componentes/modal/#como-utilizar)