📊 Portal de Notícias - Jornalizando Dados
Portal dinâmico para curadoria, rastreamento, análise e publicação de notícias sobre Análise de Dados, Marketing Digital, Tecnologia e Inovação, desenvolvido em PHP com dashboard visual e painel admin.
Automatize sua gestão de notícias com SEO, filtros avançados, coleta automática e painel moderno!

🚀 Funcionalidades Principais
Coleta Automática de Notícias (Crawler de feeds RSS e integração com Google Custom Search para imagens)

Painel Admin Completo

Dashboard visual com indicadores (notícias rastreadas, aprovadas, excluídas, pendentes, etc.)

Aprovação/desaprovação e exclusão em lote

Edição rápida (inline ou modal) de notícias (título, descrição, imagem)

Pré-visualização antes de publicar

Histórico de ações (log por usuário, aprovação, exclusão, edição)

Filtros avançados: busca por fonte, palavra-chave, data, status, presença de imagem

Dashboard de gráficos (Fontes, keywords, evolução)

Coleta manual (botão "Rodar Coleta Agora")

Publicação de Notícias

Interface moderna (Tailwind CSS)

Top News, Notícias Recentes e Populares automáticos

Suporte a imagens (original do RSS, fallback do Google ou placeholder)

SEO-friendly URLs (via .htaccess)

Scroll infinito e carregamento rápido

Arquitetura modular

Navbar e componentes reutilizáveis em PHP (include)

Separação entre frontend (usuário) e backend (admin)

🛠 Tecnologias Utilizadas
PHP (Procedural e modular)

MySQL (armazenamento de notícias, usuários, logs)

Tailwind CSS + CSS customizado

JavaScript (fetch API, AJAX, modais, scroll infinito)

Google Custom Search API (autoimagem para notícias sem thumbnail)

.htaccess (URLs amigáveis e roteamento)

Admin painel customizado (sem frameworks pesados)

📁 Estrutura de Pastas (Sugerida)
bash
Copiar
Editar
/public_html
  /noticias
    admin_painel.php
    admin_login.php
    coletar_noticias.php
    api_noticias.php
    custom.css
    ...
  /blog
    /analise-de-dados
    /marketing-digital
    /tecnologia-inovacao
    /jornalismo-de-dados
      Blog1.html ...
    index.php
  /componentes
    navbar.php
    footer.php
  .htaccess
  README.md
⚡️ Como usar
1. Clonar e Configurar o Projeto
bash
Copiar
Editar
git clone https://github.com/seu-usuario/seu-repo.git
2. Configurar Banco de Dados
Crie o banco MySQL.

Execute o script de criação das tabelas:

noticias

noticias_excluidas

usuarios

log_acoes (para histórico)

3. Configurar credenciais
Edite os arquivos PHP com as credenciais do seu banco:

php
Copiar
Editar
$host = 'localhost';
$user = 'usuario';
$pass = 'senha';
$dbname = 'banco';
4. Configurar Google Custom Search (opcional para imagens)
Criar API KEY

Criar mecanismo CX

Adicione suas chaves no coletar_noticias.php.

5. Ajustar URLs amigáveis
Edite o arquivo .htaccess (veja exemplos de rewrite no projeto).

6. Acessar o Painel Admin
/noticias/admin_login.php

Faça login, aprove as notícias, edite, exclua ou rode a coleta.

7. Personalizar Navbar/Componentes
Edite /componentes/navbar.php para manter um header global em todas as páginas.

🧩 Funcionalidades extras e Diferenciais
Curadoria semi-automatizada (auto-aprovação por keyword)

Logs e rastreabilidade (saiba quem editou/aprovou/excluiu cada notícia)

Modularidade e fácil manutenção

Dashboard visual pronto para BI (evolução, fontes, etc)

Pronto para escalar (mais fontes, mais filtros, multiusuário)

📝 Contribua!
Pull requests são bem-vindos. Para mudanças grandes, abra uma issue primeiro para discutir o que você gostaria de mudar.

📄 Licença
MIT

