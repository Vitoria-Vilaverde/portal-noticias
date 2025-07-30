Descrição do Projeto: Portal de Notícias com Painel Admin em PHP
Resumo do Projeto
Este projeto consiste em um portal de notícias totalmente dinâmico, desenvolvido em PHP e MySQL, focado em temas de Análise de Dados, Marketing Digital, Tecnologia e Inovação.
O objetivo foi criar uma plataforma onde todo o fluxo – da coleta automática das notícias até a aprovação, edição e publicação – pudesse ser feito de forma simples, visual e automatizada, com painel de controle, filtros inteligentes, dashboard visual e recursos de SEO.

Como foi o desenvolvimento
1. Levantamento dos requisitos

O sistema deveria rastrear automaticamente diversas fontes de notícias (via RSS), coletando títulos, descrições, links, datas e imagens.

Necessidade de um painel admin para curadoria (aprovar, editar, excluir notícias, etc.).

URLs amigáveis, dashboard com indicadores e busca/filtro avançado.

2. Arquitetura e organização

Organização das notícias em categorias e subpastas (ex: /blog/analise-de-dados, /blog/marketing-digital).

Estrutura modular com arquivos PHP reutilizáveis (navbar, footer, painel admin, scripts de coleta, API de notícias).

3. Coleta de notícias

Foi implementado um crawler RSS em PHP, que lê diariamente feeds configurados e armazena as notícias no banco de dados.

Quando a notícia não possui imagem, o sistema busca uma imagem correlacionada usando a API do Google Custom Search.

O painel admin permite rodar a coleta manualmente (“Rodar Coleta Agora”).

4. Painel Administrativo

Desenvolvido um painel administrativo responsivo, com login, lista de notícias rastreadas e filtros por status, fonte, palavra-chave e data.

É possível aprovar, desaprovar, excluir e editar notícias em lote, além de editar rapidamente qualquer campo via modal.

O sistema registra logs de aprovações, edições e exclusões para histórico.

5. Exibição e front-end

A interface principal utiliza Tailwind CSS e componentes em PHP para facilitar a manutenção visual.

As notícias são exibidas separadas em “Top News”, “Notícias Recentes” e “Populares”, todas geradas dinamicamente.

Imagens são exibidas automaticamente, e quando não há imagem é utilizado um placeholder.

Implementado scroll infinito para as notícias recentes.

6. URLs Amigáveis e Estrutura de Pastas

Utilizado .htaccess para criar URLs amigáveis e mover os blogs para subpastas de categoria.

Cada categoria tem sua própria página índice, facilitando a organização e navegação do site.

7. Indicadores e Dashboard

O painel exibe indicadores de total de notícias, aprovadas, pendentes, excluídas e permite visualização de gráficos de evolução das notícias e ranking de fontes.

Diferenciais
Automação da curadoria: autoaprovação de notícias por palavra-chave, coleta automatizada e manual.

Gestão visual: dashboard com indicadores e gráficos, painel amigável, filtros avançados.

Modularidade: componentes reutilizáveis em PHP, fácil manutenção, URLs SEO-friendly.

Registro de histórico: log de ações de cada usuário/admin para rastreabilidade.

Integração com Google Images: para enriquecer visualmente notícias sem imagem.

Principais aprendizados
Estruturar projetos PHP com visão de futuro (modularidade, reuso).

Automatizar coleta e curadoria, reduzindo o esforço manual.

A importância do SEO e da organização de URLs para portais de conteúdo.

Adoção de painéis visuais para facilitar a tomada de decisão do administrador.

Esse projeto demonstra como é possível unir automação, curadoria e experiência visual para criar um portal de notícias escalável, moderno e fácil de gerenciar.
