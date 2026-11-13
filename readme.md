# StudyFlow

> Organize seus estudos de forma simples.

Página web (front-end) que apresenta o **StudyFlow**, um sistema para organizar matérias, prazos e sessões de estudo em um só lugar.

## 1. Identificação do projeto

| Item | Informação |
|---|---|
| **Nome do projeto** | StudyFlow |
| **Integrantes da equipe** | Dan Rangel, Davi Martins Silva Oliveira e Bruno Félix |
| **Curso e turma** | Turma IFTP |
| **Unidade curricular** | Versionamento e colaboração (Atividade 10 – Documentação) |
| **Professor responsável** | Josué Rodrigo Evangelista Figueirêdo |

## 2. Apresentação do projeto

**O que é o projeto?**
O StudyFlow é uma página web de apresentação e painel de estudos, criada com HTML e CSS na unidade curricular de projeto front-end. Ela mostra como seria a interface de um sistema de organização de estudos voltado a estudantes.

**Qual é o principal objetivo?**
Apresentar, de forma visual e simples, uma interface em que o estudante acompanha matérias, prazos e progresso semanal em um só lugar.

**Qual problema ele busca resolver?**
Estudantes, principalmente os que se preparam para provas como o ENEM, costumam ter prazos, matérias e metas espalhados em cadernos, mensagens e aplicativos diferentes. Isso dificulta saber o que estudar, o que está atrasado e quanto já foi feito. O StudyFlow propõe reunir essas informações em uma única tela.

**Por que esse projeto foi desenvolvido?**
Para praticar, na prática, a construção de uma página front-end completa (estrutura semântica, formulário, tabela, estilização, layout flexível e responsividade) a partir de uma ideia útil para o dia a dia de estudantes.

## 3. Funcionalidades

> Esta versão é uma **interface estática**: não há JavaScript nem servidor. Os dados exibidos (prazos, matérias, porcentagens) são exemplos fixos escritos no próprio HTML. Abaixo estão apenas as funcionalidades que existem de fato.

O que o usuário consegue ver e fazer na página:

- **Navegar pelo cabeçalho:** menu com os links *Início*, *Matérias*, *Planos* e *Ajuda* (por enquanto os links ainda não levam a outras seções) e botões *Entrar* e *Cadastrar* (ainda sem ação).
- **Ver o formulário de cadastro:** campos de nome, e-mail e senha, seleção entre *Criar conta* e *Entrar* e botão *Enviar Cadastro*. O formulário é apenas visual; os dados não são enviados nem salvos.
- **Ler a proposta do sistema:** texto de apresentação, chamada "Organize sua rotina" e botões *Começar agora* e *Ver demonstração* (ainda sem ação).
- **Ver cartões de destaque:** números de exemplo (estudantes ativos, taxa de satisfação e economia de tempo por semana).
- **Consultar a "Visão geral"**, com três painéis de exemplo:
  - **Próximos Prazos:** lista de prazos, com destaque em vermelho para o que vence hoje.
  - **Matérias de hoje:** lista com status *Concluído* ou *Pendente*.
  - **Progresso da Semana:** meta de horas, porcentagem em gráfico circular e barras de estudo por dia da semana.
- **Consultar a tabela de Planos:** recursos incluídos no sistema.
- **Usar em telas diferentes:** o layout se adapta a celulares e telas pequenas (regras `@media` no CSS).
- **Ver o rodapé** com contato e direitos autorais.

## 4. Tecnologias utilizadas

| Tecnologia / ferramenta | Uso no projeto |
|---|---|
| **HTML5** | Estrutura da página (`header`, `nav`, `main`, `section`, `footer`, formulário, tabela). |
| **CSS3** | Estilização, cores, Flexbox, cartões, gráfico circular com `conic-gradient` e responsividade com `@media`. |
| **Visual Studio Code** | Editor de código usado no desenvolvimento. |
| **Git e GitHub** | Versionamento e publicação do projeto. |

Não foram usadas bibliotecas, frameworks nem JavaScript. O CSS está dentro do próprio arquivo HTML, na tag `<style>`.

## 5. Estrutura do projeto

```
studyflow/
├── studyflow.html      # Página completa: estrutura (HTML) e estilos (CSS)
├── README.md           # Esta documentação
└── imagens/            # Capturas de tela usadas na demonstração
```

| Arquivo / pasta | Finalidade |
|---|---|
| `studyflow.html` | Único arquivo do sistema. Contém o HTML da página e o CSS dentro da tag `<style>`. |
| `README.md` | Documentação do projeto, exibida na página inicial do repositório. |
| `imagens/` | Capturas de tela da página, usadas na seção de demonstração. |

## 6. Como executar o projeto

Não é preciso instalar nada além de um navegador moderno (Chrome, Edge, Firefox etc.).

1. Baixe o projeto (botão **Code → Download ZIP** no GitHub) ou clone o repositório: `git clone <link-do-repositorio>`.
2. Se baixou o ZIP, extraia a pasta.
3. Dê um duplo clique em `studyflow.html` para abri-lo no navegador.

Opcional: no Visual Studio Code, abra a pasta do projeto e use a extensão *Live Server* para ver as alterações em tempo real.

## 7. Demonstração do projeto

**Cabeçalho com logotipo, menu de navegação e botões de acesso.**
![Cabeçalho do StudyFlow](imagens/01-cabecalho.png)

**Formulário de cadastro, com nome, e-mail, senha e escolha entre criar conta ou entrar.**
![Formulário de cadastro](imagens/02-cadastro.png)

**Cartões de destaque com números de exemplo.**
![Cartões de destaque](imagens/03-destaques.png)

**Visão geral: próximos prazos, matérias de hoje e progresso da semana.**
![Visão geral](imagens/04-visao-geral.png)

**Tabela de planos com os recursos incluídos.**
![Tabela de planos](imagens/05-planos.png)

**Rodapé com contato e direitos autorais.**
![Rodapé](imagens/06-rodape.png)

**Página completa no computador.**
![Página completa no desktop](imagens/07-pagina-completa-desktop.png)

**Página em tela de celular, mostrando a adaptação do layout.**
![Versão para celular](imagens/08-versao-celular.png)

## 8. Melhorias futuras

1. **Tornar o cadastro e o login funcionais:** com JavaScript e um back-end (ou serviço de autenticação), validar os campos, guardar os usuários e proteger a senha. Hoje o campo de senha mostra o texto digitado; o ideal é usar `type="password"`.
2. **Permitir cadastrar e editar prazos e matérias:** hoje os dados são fixos. Com JavaScript e armazenamento (como `localStorage` ou banco de dados), o usuário poderia criar, concluir e remover tarefas, e o progresso semanal seria calculado automaticamente.
3. **Ativar a navegação e os botões:** fazer os links do menu levarem às seções, criar páginas separadas (Matérias, Planos, Ajuda) e dar função aos botões *Entrar*, *Cadastrar*, *Começar agora* e *Ver demonstração*.
4. **Notificações, calendário e simulados:** lembretes de estudo, calendário para marcar dias de estudo e provas, e simulados no modelo ENEM ou vestibular.
5. **Melhorar acessibilidade e organização do código:** separar o CSS em um arquivo próprio (`style.css`), melhorar o contraste de cores e a navegação por teclado.
6. **Substituir os números de exemplo por dados reais:** os cartões "12k+ estudantes" e "98% de satisfação" são ilustrativos e devem ser trocados quando houver dados verdadeiros.
