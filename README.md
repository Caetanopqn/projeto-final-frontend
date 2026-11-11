# DevCompass

Site guia para orientar estudantes de TI na preparação para o mercado de trabalho.

**Autor:** Caetano Pequeno

**Disciplina:** Desenvolvimento Front-End para web

**Ano:** 2026

---

## Sobre o projeto

O DevCompass funciona como uma bússola para estudantes de Tecnologia da Informação. Ele ajuda a decidir o que estudar, o que desenvolver e o que criar para se preparar para o mercado de trabalho em uma área específica de TI, com foco na busca pelo primeiro estágio.

A plataforma organiza as etapas dessa preparação em trilhas de aprendizagem e projetos para portfólio. Cada uma dessas funcionalidades muda de acordo com a área de TI escolhida pelo usuário.

O site também permite criar planos de estudo e acompanhar o progresso e as atividades.

## Objetivos

- Ajudar o estudante a escolher uma área de atuação em TI.
- Indicar trilhas de aprendizagem e cursos relacionados a cada área.
- Sugerir projetos que ajudem a criar e ampliar o portfólio.
- Acompanhar o progresso do estudante em cursos e metas diárias.
- Aplicar na prática os conceitos de HTML e CSS vistos na disciplina.

## Telas

### Login (`login.html`)
Tela de acesso ao sistema.

### Dashboard (`painel.html`)
Visão geral do estudante, com:
- Cards de resumo: lições em progresso, lições concluídas e conquistas.
- Gráfico de horas gastas nos últimos 7 dias, feito apenas com HTML e CSS.
- Indicador de performance com barra de progresso.
- Lista de cursos em andamento, com porcentagem de conclusão.

### Trilhas (`trilhas.html`)
Catálogo de trilhas de aprendizagem. O usuário escolhe uma área (por exemplo, Desenvolvimento Web, Dados e IA ou Cibersegurança) e a página mostra apenas as trilhas daquela área, com nível, carga horária, quantidade de cursos e progresso.

### Projetos (`projetos.html`)
Catálogo de ideias de projetos para o portfólio, com filtro por área. Cada projeto informa o nível, as tecnologias envolvidas, o tempo estimado e onde publicar o resultado.

## Tecnologias utilizadas

- HTML5
- CSS3 (Flexbox, Grid, variáveis CSS e o seletor `:has`)
- [Boxicons](https://boxicons.com/) para os ícones
- [Google Fonts](https://fonts.google.com/) (fonte Raleway)

## Como executar

1. Baixe ou clone o repositório.
2. Abra a pasta do projeto em um editor de código.
3. Abra o arquivo `painel.html` no navegador, ou use uma extensão como o Live Server.

Os arquivos CSS são carregados com caminhos que começam com barra (`/css/painel.css`), que dependem de um servidor local. Se abrir o HTML diretamente pelo arquivo e os estilos não carregarem, use o Live Server ou troque os caminhos para relativos (`../css/painel.css`).

## Decisões técnicas

- **Layout com Grid e Flexbox:** o Grid organiza áreas com colunas definidas (cards de resumo, gráfico e performance), e o Flexbox alinha os itens dentro de cada card.
- **Gráfico sem bibliotecas:** a altura de cada barra do gráfico vem de uma variável CSS (`--h`), definida no próprio HTML.
- **Barras de progresso:** feitas com o elemento nativo `<progress>`, estilizado para Chrome, Edge, Safari e Firefox.
- **Filtros sem JavaScript:** os seletores de área usam campos `radio` escondidos junto com o seletor `:has`, que mostram ou escondem os cards de acordo com a área escolhida.
- **Reaproveitamento de estilos:** o arquivo `painel.css` guarda o reset, o fundo, os cards, os botões e a barra de progresso, e as demais telas apenas acrescentam o que é específico delas.

## Compatibilidade

O filtro por área depende do seletor `:has`, que funciona nas versões atuais dos principais navegadores. Em navegadores antigos, todos os cards podem ser exibidos ao mesmo tempo.

## Próximos passos

- Desenvolver o criador de planos de estudo.
- Criar a página interna de cada trilha, com a lista de cursos.
- Adicionar JavaScript para guardar a área escolhida e o progresso do usuário.

## Autor

Caetano Pequeno

Disciplina de Desenvolvimento Front-End para web, 2026.
