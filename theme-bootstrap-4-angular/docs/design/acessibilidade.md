[Skip to main content](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#docusaurus_skipToContent_fallback)

On this page

"Somente 2% das páginas web governamentais são acessíveis." “É obrigatória a acessibilidade nos sites da internet mantidos por empresas com sede ou representação comercial no País ou por órgãos de governo, para uso da pessoa com deficiência, garantindo-lhe acesso às informações disponíveis, conforme as melhores práticas e diretrizes de acessibilidade adotadas internacionalmente.” Lei Nº 13.146

A proposta de um website (ou qualquer outra mídia digital) bem concebido e acessível é a de beneficiar as pessoas com necessidades especiais, dando-lhes autonomia e permitindo que elas não só utilizem, mas também contribuam com a web.

Sua flexibilidade beneficia igualmente pessoas idosas, aquelas não fluentes na escrita de um idioma, pessoas com conexões lentas, ou usuários de tecnologias ultrapassadas, internautas novos ou pouco frequentes, usuários de telefones móveis, indivíduos com limitações temporárias, entre outros.

Um website com adequado contraste de cores e com opção para alternância de tamanho da fonte beneficia igualmente o indivíduo com baixa visão, com a visão comprometida pela idade e quem faz uma busca em seu celular à luz do sol, por exemplo.

O Design universal significa um grande passo na direção de um mundo cada vez mais inclusivo, que se adapta cada vez mais às diferentes habilidades e necessidades das pessoas e que exige delas cada vez menos esforço individual adaptativo, o qual, como sabemos, acaba sempre por excluir muitas pessoas da participação na vida social e também por privar a sociedade da contribuição que poderia ser trazida por essas pessoas.

São sete os princípios do Design universal:

1. **Equiparação nas possibilidades de uso**: pode ser utilizado por qualquer usuário em condições equivalentes.
2. **Flexibilidade de uso**: atende a uma ampla gama de indivíduos, preferências e habilidades individuais.
3. **Uso simples e intuitivo**: fácil de compreender, independentemente da experiência do usuário, de seus conhecimentos, aptidões linguísticas ou nível de concentração.
4. **Informação perceptível**: fornece de forma eficaz a informação necessária, quaisquer que sejam as condições ambientais/físicas existentes ou as capacidades sensoriais do usuário.
5. **Tolerância ao erro**: minimiza riscos e consequências negativas decorrentes de ações acidentais ou involuntárias.
6. **Mínimo esforço físico**: pode ser utilizado de forma eficiente e confortável, com um mínimo de fadiga.
7. **Dimensão e espaço para uso e interação**: espaço e dimensão adequados para a interação, o manuseio e a utilização, independentemente da estatura, da mobilidade ou da postura do usuário.

Assim, a partir de uma web acessível, muitos cenários aparentemente improváveis tornam-se possíveis, não só para pessoas com deficiência, mas também para qualquer categoria de usuário, tais como:

- Uma mulher cega, utilizando um leitor de telas, pesquisa a restituição de imposto de renda no site da Receita Federal;
- Um homem com paralisia cerebral, com grandes dificuldades motoras e que só utiliza um dedo para teclar, atualiza seu perfil em uma rede social;
- Um homem com deficiência motora, que usa um mouse adaptado, faz compras em uma loja virtual;
- Uma jovem tetraplégica, utilizando apenas um ponteiro na cabeça, procura informações sobre células-tronco em sítios especializados;
- Uma mulher com deficiência intelectual faz exercícios pela web para melhorar sua comunicação;
- Um senhor surdocego namora pela web, utilizando um dispositivo que mostra em Braille as informações exibidas na tela;
- Uma mulher com baixa visão procura informações sobre investimentos e a crise econômica mundial, utilizando um programa ampliador de tela;
- Um programador daltônico testa uma aplicação na web, procurando erros;
- Um jovem surdo ou com deficiência auditiva que faz um curso de inglês à distância;
- Um homem cego e sem braços procura sua ex-professora em um sistema de busca utilizando um programa de reconhecimento de voz para entrar comandos no computador e receber retorno a partir do leitor de telas;
- Uma jovem com dificuldade de leitura, em virtude da combinação de transtorno do déficit de atenção com hiperatividade (TDAH) e dislexia, estudante do ensino médio, que gosta das aulas de literatura complementa a leitura de livros e estudos por meio de aulas on-line. Ela utiliza um programa que realça o texto na tela, ao mesmo tempo em que é realizada uma leitura em voz alta.
- Um funcionário do governo precisa rever dados importantes no caminho de uma viagem e tem apenas celular à disposição;
- No meio de um pregão eletrônico falta energia e os funcionários utilizam um tablet com conexão 3G para continuar;
- Em um município do interior, a escola precisa enviar os dados dos alunos, mas só contam com conexão 2G.

Fonte: [Acesso para todos](https://www.acessoparatodos.com.br/acessibilidadeweb.php), [W3C](https://www.w3c.br/pub/Materiais/PublicacoesW3C/cartilha-w3cbr-acessibilidade-web-fasciculo-I.html), [Cartilha W3C](https://www.w3c.br/Materiais/materiais/cartilha-w3cbr-acessibilidade-web-fasciculo-III.html), [Lei 13146](http://www.planalto.gov.br/ccivil_03/_Ato2015-2018/2015/Lei/L13146.htm)

## Leitores de tela [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#leitores-de-tela "Direct link to Leitores de tela")

- o site precisa ter hierarquia bem definida, com header, nav, section, article, aside e footer. [Fonte](http://emag.governoeletronico.gov.br/#s3)
- precisa usar alt e titles
- precisa usar os aria- .... [Fonte](https://www.w3.org/TR/2021/WD-html-aria-20210328/)
- Links indefinidos
- Não usar carregamento automático
- Tabelas precisam de contexto no código
- precisa ser responsivo com crtl + e - (responsivo resolve)
- cuidar pseudo elementos por não serem lidos por SR

### Deficiência física [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#defici%C3%AAncia-f%C3%ADsica "Direct link to Deficiência física")

- Espaçamento de padding nos elementos clicáveis
- Espaçamento de respiro entre os elementos

### Contraste [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#contraste "Direct link to Contraste")

De acordo com o Guia de Acessibilidade para Conteúdo Web do W3C
( [WCAG](https://www.w3.org/Translations/WCAG20-pt-PT/), em inglês), a
taxa de contraste mínima (nível AA) para textos normais (até 18px) é de
4.5:1, e 3:1 para textos grandes (acima de 18px). Para garantir a
acessibilidade dos recursos disponibilizados na interface dos produtos,
é necessário verificar a taxa de contraste das cores utilizadas. Para
tanto, recomenda-se a utilização da ferramenta disponível neste
[link](https://webaim.org/resources/contrastchecker/).

Saiba mais em [Fundamentos de Cores](https://docs.plataforma.betha.cloud/docs/design/fundamentos/cores).

### Daltonismo [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#daltonismo "Direct link to Daltonismo")

Não basear informações apenas em cores. Sempre utilizar texto, ícones ou texturas para diferenciar estados ou opções diferentes.

##### Certo

Azul

Amarelo

##### Errado

## Ergonomia [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#ergonomia "Direct link to Ergonomia")

LER, idosos e uma mão

## Responsividade [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#responsividade "Direct link to Responsividade")

## Cognição [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#cogni%C3%A7%C3%A3o "Direct link to Cognição")

- Não usar captcha
- Não sobrecarregar cognição
- Linhas de leitura muito extensas ou justificadas
- Elementos muito pequenos

## Texto [​](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/\#texto "Direct link to Texto")

O texto de um sistema ou site deve ser de fácil leitura e compreensão, não exigindo do usuário um nível de instrução mais avançado do que o ensino fundamental completo. Quando o texto exigir uma capacidade de leitura mais avançada, deve ser disponibilizado informações suplementares que expliquem ou ilustrem conteúdo principal. Outra alternativa é versão simplificada do conteúdo em texto.

Existem algumas técnicas que auxiliam na melhora da inteligibilidade de textos, como, por exemplo:

1. Desenvolver apenas um tópico por parágrafo;
2. Utilizar sentenças organizadas de modo simplificado para o propósito do conteúdo (sujeito, verbo e objeto, preferencialmente);
3. Dividir sentenças longas em sentenças mais curtas;
4. Evitar o uso de jargão, expressões regionais ou termos especializados que possam não ser claros para todos;
5. Utilizar palavras comuns no lugar de outras pouco familiares;
6. Utilizar listas de itens ao invés de uma longa série de palavras ou frases separadas por vírgulas;
7. Fazer referências claras a pronomes e outras partes do documento;
8. Utilizar, preferencialmente, a voz ativa.

Fonte: [Emag](http://emag.governoeletronico.gov.br/#r21_b)

- [Leitores de tela](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#leitores-de-tela)
  - [Deficiência física](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#defici%C3%AAncia-f%C3%ADsica)
  - [Contraste](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#contraste)
  - [Daltonismo](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#daltonismo)
- [Ergonomia](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#ergonomia)
- [Responsividade](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#responsividade)
- [Cognição](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#cogni%C3%A7%C3%A3o)
- [Texto](https://docs.plataforma.betha.cloud/docs/design/acessibilidade/#texto)