[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/layout/grid/#docusaurus_skipToContent_fallback)

On this page

O sistema de grid é a base estrutural da organização dos elementos das interfaces. São organizados por meio de um `.container` que abriga uma série de linhas `.row` e colunas `.col-`, que recebem os componentes.

![Ilustração](https://docs.plataforma.betha.cloud/img/grid.svg)

## Container [​](https://docs.plataforma.betha.cloud/docs/design/layout/grid/\#container "Direct link to Container")

É utilizado para agrupar o conteúdo da interface e garantir a responsividade e a fluidez de seus elementos. Utiliza-se como pai dos outros elementos na tela para organizá-los.
Existem duas variações para o container:

### Container limitado [​](https://docs.plataforma.betha.cloud/docs/design/layout/grid/\#container-limitado "Direct link to Container limitado")

`.container` Limita a largura dos elementos da interface.![Ilustração](https://docs.plataforma.betha.cloud/img/container.png)

### Container fluido [​](https://docs.plataforma.betha.cloud/docs/design/layout/grid/\#container-fluido "Direct link to Container fluido")

`.container-fluid` Permite que os elementos da interface extendam-se à largura da tela.![Ilustração](https://docs.plataforma.betha.cloud/img/container-fluid.png)

## Linha [​](https://docs.plataforma.betha.cloud/docs/design/layout/grid/\#linha "Direct link to Linha")

As linhas de classe `.row` são indispensáveis, pois abrigam as divs de colunas. Uma linha corresponde ao espaço de 12 colunas.

Uma linha `.row` não deve ser colocada diretamente dentro de outra linha `.row`.

As linhas `.row` possuem comportamento flex por padrão, podendo serem acompanhadas por [classes de alinhamento](https://docs.plataforma.betha.cloud/docs/design/layout/alinhamento) horizontais e verticais.

## Colunas [​](https://docs.plataforma.betha.cloud/docs/design/layout/grid/\#colunas "Direct link to Colunas")

São as classes que expressam quantas colunas irão ocupar no grid. Elas podem variar de `.col-1` a `.col-12`.

Elas também podem assumir comportamento responsivo, alterando o grid em determinado tamanho de dispositivo:

- `.col-` (até 576px) smartphones;
- `.col-sm-` (576px ou maior) tablets ;
- `.col-md-` (768px ou maior) computadores antigos;
- `.col-lg-` (992px ou maior) computadores modernos;

**Nota**: A variação responsiva da coluna será a mesma daquele tamanho em diante, caso outra não seja adicionada. Por exemplo: Se apenas a classe "col-12" for especificada, esse será o tamanho da coluna em todos os dispositivos.

## Exemplo [​](https://docs.plataforma.betha.cloud/docs/design/layout/grid/\#exemplo "Direct link to Exemplo")

- Vanilla

```html
<div class="container">
    <div class="row">
        <div class="col-12 col-sm-6 col-lg-4" id="d1">...</div>
        <div class="col-12 col-sm-6 col-lg-4" id="d2">...</div>
        <div class="col-12" id="d3">
            <div class="row">
                <div class="col-6">...</div>
                <div class="col-6">...</div>
            </div>
        </div>
    </div>
</div>
```

Note que as divs " **d1**" e " **d2**" irão preencher todo o espaço horizontal no smartphone, metade em tablets e computadores antigos, e 1/3 em computadores modernos. Já a div " **d3**" preencherá o espaço completo da linha `.row` em todos os dispositivos.

- [Container](https://docs.plataforma.betha.cloud/docs/design/layout/grid/#container)
  - [Container limitado](https://docs.plataforma.betha.cloud/docs/design/layout/grid/#container-limitado)
  - [Container fluido](https://docs.plataforma.betha.cloud/docs/design/layout/grid/#container-fluido)
- [Linha](https://docs.plataforma.betha.cloud/docs/design/layout/grid/#linha)
- [Colunas](https://docs.plataforma.betha.cloud/docs/design/layout/grid/#colunas)
- [Exemplo](https://docs.plataforma.betha.cloud/docs/design/layout/grid/#exemplo)