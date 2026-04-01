Este projeto é um aplicativo de gerenciamento de pessoas (CRUD) desenvolvido para facilitar o cadastro, edição, visualização e exclusão de usuários. 
O foco principal foi criar uma interface simples e funcional para dispositivos móveis e web, permitindo o armazenamento persistente de dados através de uma API simulada.

Tecnologias Utilizadas:

  React Native / Expo: Framework para o desenvolvimento da interface e navegação.

  JavaScript: Linguagem base para a lógica do sistema.

  JSON-Server: Utilizado para simular uma API REST e gerenciar o banco de dados local.

  React Navigation: Para a transição entre a tela de listagem e a tela de formulário.

A solução foi estruturada separando a interface (Frontend) da persistência de dados (Mock API).

  Comunicação: Criei um módulo de serviços (peopleCrud.js) que centraliza todas as requisições HTTP (GET, POST, PUT, DELETE) usando a API fetch.

  Estado: O aplicativo utiliza o useState para gerenciar os dados em tempo real e o useEffect para carregar a lista de pessoas sempre que a tela inicial é aberta.

  Navegação: Implementei uma Stack Navigation para separar a visualização dos dados da área de edição, garantindo que o usuário possa voltar e avançar sem perder o contexto.

  Backend: O json-server observa o arquivo db.json, funcionando como um banco de dados real que mantém as informações gravadas mesmo após fechar o aplicativo.

Instalação:

Pré-requisito:

  Node.js instalado.

No terminal: 

  cd meuCrudApp
  npm install

e
  cd crud-server
  npm install json-server

Execução: 

No terminal:

  cd crud-server
  npx json-server --watch db.json --port 3000

  cd meuCrudApp
  npx expo start --web

  
