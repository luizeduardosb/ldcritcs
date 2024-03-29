# LDCritcs - Site de Críticas de Jogos de Videogame

*Este é um repositório secundário, apenas de demonstração. O repositório original, com todos os commits e movimentações do projeto, segue privado.

*Para utilizar o projeto será necessário ter o Play Framework instalado em sua máquina.

O LDCritcs é um projeto pessoal de aplicação web dedicada à análise e críticas de jogos de videogame. 
Este repositório contém o código-fonte completo do projeto.

Acesse meu linkedin para mais informações: https://www.linkedin.com/in/luiz-bezerra-80355a298/

##Tecnologias utiizadas:
Java | Play Framework | JavaScript | ViaCEP API | HTML5 | CSS3 | Bootstrap | Figma 


## Funcionalidades Principais

- **Carrossel de Destaques:** Destaques de jogos populares são exibidos em um carrossel na página inicial, cada um acompanhado de uma breve descrição.
- **Seleção de Plataformas:** Os usuários podem filtrar os jogos por plataforma, incluindo opções para Xbox, PlayStation, Windows e Switch.
- **Lista de Jogos:** Uma lista de jogos completa com detalhes, incluindo nome, desenvolvedor, gênero, plataforma e descrição.
- **Avaliação Média:** Mostra a avaliação média de cada jogo, baseada em críticas e pontuações dos usuários.
- **Notícias de Jogos:** Uma seção de notícias de jogos apresenta as últimas novidades do mundo dos videogames.
- **Funcionalidades Administrativas:** Para administradores logados, há a possibilidade de editar e excluir jogos diretamente do site.


Abaixo estão informações adicionais sobre os principais controllers do projeto:

### `controllers.Criticas`
Este controller lida com operações relacionadas às críticas dos jogos. Suas principais funcionalidades incluem:
- Exibir um formulário para submissão de críticas.
- Salvar uma crítica no banco de dados.
- Listar críticas existentes, permitindo a busca por palavras-chave.
- Editar críticas existentes.

### `controllers.Games`
O controller Games gerencia operações relacionadas aos jogos. Suas funcionalidades incluem:
- Exibir a página inicial com a lista de jogos e críticas associadas.
- Permitir a adição, edição e exclusão de jogos.
- Exibir detalhes de um jogo específico, incluindo todas as críticas associadas.
- Calcular a nota média de um jogo com base nas críticas recebidas.
- Remover uma crítica específica associada a um jogo.

### `controllers.Seguranca`
Este controller cuida das questões de segurança da aplicação. Suas principais funcionalidades incluem:
- Garantir que o usuário esteja autenticado antes de acessar certas páginas.
- Verificar se o usuário possui privilégios de administrador antes de realizar ações específicas.


### `controllers.Usuarios`
Este controller é responsável por lidar com operações relacionadas aos usuários do sistema. Suas principais funcionalidades incluem:
- Controle de todos os usuários, como deletar, salvar e editar.
- Validações de registro, como garantir que o perfil padrão seja "comum" e que o nome de usuário contenha um "@".
- O login autentica um usuário com base no nome de usuário e senha fornecidos. Se as credenciais estiverem corretas, o usuário é redirecionado para a página inicial do sistema. Caso contrário, uma mensagem de erro é exibida.
- A validação de login exibe uma mensagem de erro quando as credenciais de login são inválidas.
- Ao clicar em sair, o sistema limpa a sessão do usuário e redireciona para a página inicial.
