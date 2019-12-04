# HUB _tasks_ - Aplicação para gerenciamento de tarefas

A aplicação está hospedada na plataforma HEROKU e pode ser acessada clicando [Aqui](https://app-hubtasks.herokuapp.com/) 
### Usuário para teste:
    email: teste@teste.com
    password: teste

Para esse usuário foram criadas algumas tasks como exemplo, mas podendo também ser criado outro usuário para testar as funcionalidades
#


Para rodar a aplicação localmente clone o projeto e digite no terminal dentro do diretório do projeto:

    docker-compose up --build -d
E acesse:
    [HUBtasks](http://localhost)
#
No desenvolvimento desse projeto foram usadas as seguintes tecnologias:
    
  - __ReactJS__ ( desenolvimento da interface Web responsiva )
  - __NodeJS__ ( desenvolvimento  da API que realiza o gerenciamento das tasks)
  - __MongoDB__ ( base de dados )

E as seguintes ferramentas:

### Docker
Usado para conteneirizar a aplicação facilitando sua execução e manutenção.

### MongoDB Atlas
Banco como serviço usado como base de dados para a aplicação
### Git Flow
Ferramenta utilizada para melhor gerenciar o versionamento do projeto ( ex: branchs, commits)
#



Diversas bibliotecas e frameworks foram usados visando otimização dos processos. 

Algumas deles foram:

#### Backend
  - __Express__: microframework utilizado para criação de aplicações web
  - __Mongoose__: espécie de object data mapping para facil manipulação dos dados fornecidos pelo banco Mongo
  
 #### Frontend
  - __Axios__: biblioteca usada para realização de chamadas REST
  - __React Router Dom__: usado para navegação entre páginas e componentes no React
  - __Redux__: provê um melhor controle da aplicação, possibilitando um melhor controle do estado global da aplicação
  - __Redux Saga__: middleware utilizado para gerenciar os side-effects da aplicação, assim como ações assíncronas.
  
  #
  ## MELHORIAS
  
 Aqui irei listar possíveis melhorias que poderiam ser feitas posteriormente com a evolução do projeto
 
 
1. Caso o backend precise ser publicamente exposto, poderia ser adicionado uma interface para documentação do mesmo, tal como SWAGGER.

2. Adicionar metodo de autenticacao com token (ex:JWT)

3. Relação entre tabelas (ex: tasks dentro de um projeto), e o projeto pode ser compartilhado entre diferentes usuários.

4. Criar uma tela com permissão para gerente (super user), onde ele teria acesso aos dados de todos os usuários e todas as tasks.

5. Adicionar as respectivas importâncias das entregas (prioridades).

6. Utilizar Styled Components, para facilitar a criação de componentes estilizados na aplicação.

7. Juntamente com a aplicação, disponibilizar um container com uma imagem do banco utilizado (Ex: mongo)

8. Segurança adicionando variáveis de ambiente importante da aplicação

9. Adicionar alguns indicadores de status (activity loader) para dar ao cliente noção de telas carregando 
  ou requisições sendo efetuadas.

10. Proporcionar ao usuário ações como resgatar tasks antigas, a funcionalidade SOFT DELETE foi implementada
no backend porém o usuário não tem conhecimento da mesma ainda. 
