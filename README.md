<p align="center">
  <img src="./public/src/assets/logo/spotify-logo.png" alt="Logo do Projeto Spotify" width="150"/>
</p>

<h1 align="center">Projeto Spotify Clone</h1>

<p align="center">
  Um clone do Spotify com front-end inteligente e player dinâmico, construído com JavaScript, React, e interagindo com uma API própria para uma experiência completa!
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js"/>
  <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>
  <img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>
  <img src="https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white" alt="ESLint"/>
</p>

<p align="center">
  <img src="https://img.shields.io/github/stars/SEU_USUARIO_GITHUB/SEU_REPOSITORIO_GITHUB?style=social" alt="GitHub Stars"/>
  <img src="https://img.shields.io/github/forks/SEU_USUARIO_GITHUB/SEU_REPOSITORIO_GITHUB?style=social" alt="GitHub Forks"/>
  <img src="https://img.shields.io/github/issues/SEU_USUARIO_GITHUB/SEU_REPOSITORIO_GITHUB?style=social" alt="GitHub Issues"/>
  </p>

---

## 📝 Sumário

* [✨ Sobre o Projeto](#-sobre-o-projeto)
* [🚀 Funcionalidades](#-funcionalidades)
* [🛠️ Tecnologias Utilizadas](#️-tecnologias-utilizadas)
* [📁 Estrutura do Projeto](#-estrutura-do-projeto)
* [🏁 Começando](#-começando)
    * [Pré-requisitos](#pré-requisitos)
    * [Instalação](#instalação)
* [📜 Scripts Disponíveis](#-scripts-disponíveis)
* [🔗 Interação com a API](#-interação-com-a-api)
* [🖼️ Telas da Aplicação](#️-telas-da-aplicação)
* [🤝 Contribuindo](#-contribuindo)
* [📄 Licença](#-licença)
* [🧑‍💻 Autor](#-autor)

---

## ✨ Sobre o Projeto

Este projeto é um clone da interface e funcionalidades básicas do Spotify, desenvolvido como parte da Jornada Full Stack. O objetivo foi criar uma aplicação web completa, desde o front-end interativo com React até o back-end com API própria e integração com banco de dados. A aplicação conta com um player de música dinâmico, listagem de artistas e músicas, e uma navegação fluida entre as páginas.

---

## 🚀 Funcionalidades

* **Interface Inspirada no Spotify:** Design familiar e intuitivo.
* **Player de Música Dinâmico:**
    * Controles de play, pause, avançar e retroceder música.
    * Barra de progresso da música.
    * Exibição de informações da música atual (nome, artista, imagem do álbum).
* **Navegação entre Páginas:**
    * Página Inicial: Exibição de artistas e músicas populares.
    * Página de Artistas: Listagem de todos os artistas.
    * Página de Detalhes do Artista: Exibição das músicas populares do artista e banner.
    * Página de Músicas: Listagem de todas as músicas.
    * Página de Detalhes da Música (Player): Foco na música selecionada com controles do player.
* **Front-end Inteligente:** Componentização com React para uma interface reativa e eficiente.
* **Back-end Robusto:**
    * API RESTful para servir os dados de artistas e músicas.
    * Conexão com banco de dados MongoDB para persistência dos dados.
* **Consumo de API:** Frontend consome dados da API desenvolvida para o projeto.
* **Responsividade (Básica):** Adaptação para diferentes tamanhos de tela (conforme `App.css`).

---

## 🛠️ Tecnologias Utilizadas

O projeto foi construído utilizando as seguintes tecnologias:

* **Front-end:**
    * [JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
    * [React](https://react.dev/) (v19)
    * [React Router DOM](https://reactrouter.com/) (v7.1.5) - Para gerenciamento de rotas.
    * [Axios](https://axios-http.com/) - Para requisições HTTP à API.
    * [Font Awesome](https://fontawesome.com/) - Para ícones.
    * HTML5
    * CSS3 (com metodologia BEM para classes)
* **Back-end:**
    * [Node.js](https://nodejs.org/) (implícito)
    * [MongoDB](https://www.mongodb.com/) - Banco de dados NoSQL.
    * Driver `mongodb` para Node.js - Para interação com o banco de dados.
* **Ferramentas de Desenvolvimento:**
    * [Vite](https://vitejs.dev/) - Build tool e servidor de desenvolvimento.
    * [ESLint](https://eslint.org/) - Para linting do código JavaScript/JSX.
* **Hospedagem:**
    * Front-end e Back-end hospedados no [Render](https://render.com/) (inferido pelo link `https://deploy-jornada-full-stack.onrender.com`).

---

## 📁 Estrutura do Projeto

---

## 📁 Estrutura do Projeto

```text
spotify-clone/
├── public/
│   └── src/assets/logo/spotify-logo.png  # Favicon e logo principal
│   └── index.html                        # Template HTML principal
├── src/                                  # Código fonte do front-end
│   ├── assets/
│   │   ├── database/                     # Dados iniciais (artists.js, songs.js)
│   │   └── logo/                         # Logo
│   ├── components/                       # Componentes React reutilizáveis
│   │   ├── Header.jsx
│   │   ├── ItemList.jsx
│   │   ├── Player.jsx
│   │   ├── SingleItem.jsx
│   │   └── SongItem.jsx
│   ├── pages/                            # Componentes de página
│   │   ├── Artist.jsx
│   │   ├── Artists.jsx
│   │   ├── Home.jsx
│   │   ├── Song.jsx
│   │   └── Songs.jsx
│   ├── App.jsx                           # Componente principal com rotas
│   ├── index.css                         # Estilos globais e reset
│   └── main.jsx                          # Ponto de entrada da aplicação React
├── server/                               # Código fonte do back-end
│   ├── connect.js                        # Configuração da conexão com MongoDB
│   ├── populate_database.js              # Script para popular o banco (se houver)
│   └── ...                               # Outros arquivos da API (rotas, controllers)
├── .env                                  # Variáveis de ambiente (ex: URI do MongoDB)
├── .eslintrc.js                          # Configuração do ESLint
├── .gitignore                            # Arquivos e pastas a serem ignorados pelo Git
├── package.json                          # Metadados do projeto e dependências
└── vite.config.js                        # Configuração do Vite

---
``` 

## 🏁 Começando

Siga estas instruções para configurar e rodar o projeto em seu ambiente local.

### Pré-requisitos

* [Node.js](https://nodejs.org/) (versão LTS recomendada)
* [npm](https://www.npmjs.com/) ou [yarn](https://yarnpkg.com/)
* Uma instância do [MongoDB](https://www.mongodb.com/try/download/community) (local ou Atlas)

### Instalação

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/SEU_USUARIO_GITHUB/SEU_REPOSITORIO_GITHUB.git](https://github.com/SEU_USUARIO_GITHUB/SEU_REPOSITORIO_GITHUB.git)
    cd SEU_REPOSITORIO_GITHUB
    ```
    2.  **Instale as dependências do Front-end (e Back-end, se estiverem no mesmo `package.json`):**
    ```bash
    npm install
    # ou
    yarn install
    ```

3.  **Configure as Variáveis de Ambiente:**
    * Crie um arquivo `.env` na raiz do projeto.
    * Adicione a URI de conexão do seu MongoDB:
        ```env
        MONGODB_URI=mongodb+srv://seu_usuario:sua_senha@seu_cluster....mongodb.net/spotifyCloneDB?retryWrites=true&w=majority
        ```
    * (Se o back-end tiver um `.env` separado na pasta `server/`, configure-o lá).

4.  **(Opcional) Popule o Banco de Dados:**
    Se houver um script para popular o banco e for necessário:
    ```bash
    node server/populate_database.js
    ```
    *(Verifique o caminho e o comando exato no seu projeto)*

5.  **Inicie o Servidor de Desenvolvimento do Front-end:**
    ```bash
    npm run dev
    # ou
    yarn dev
    ```
    Acesse `http://localhost:5173` (ou a porta indicada pelo Vite) no seu navegador.

6.  **Inicie o Servidor Back-end:**
    (O comando exato dependerá de como seu servidor está configurado. Exemplo comum:)
    ```bash
    node server/index.js
    # ou o script definido no package.json para o backend, se houver.
    ```
    A API estará disponível em `http://localhost:PORTA_BACKEND` (verifique a porta configurada no seu backend, por exemplo, `http://localhost:3000/api`).

---

## 📜 Scripts Disponíveis

No diretório raiz do projeto, você pode executar vários scripts:

* `npm run dev` ou `yarn dev`:
    Inicia o servidor de desenvolvimento do Vite para o front-end com hot-reloading.

* `npm run build` ou `yarn build`:
    Compila a aplicação React para produção na pasta `dist/`.

* `npm run lint` ou `yarn lint`:
    Executa o ESLint para verificar erros de formatação e padrões de código.

* `npm run preview` ou `yarn preview`:
    Inicia um servidor local para visualizar a build de produção.

---

## 🔗 Interação com a API

O front-end realiza chamadas para uma API própria para buscar e interagir com os dados. Os principais endpoints consumidos são:

* `GET /api/artists`: Retorna a lista de todos os artistas.
* `GET /api/songs`: Retorna a lista de todas as músicas.
* `GET /api/artists/:id`: Retorna detalhes de um artista específico (implícito).
* `GET /api/songs/:id`: Retorna detalhes de uma música específica (implícito).

A URL base da API em produção é: `https://deploy-jornada-full-stack.onrender.com/api`

---

## 🖼️ Telas da Aplicação

_(Adicione aqui screenshots/GIFs do seu projeto para torná-lo mais visual e atrativo)_

* **Página Inicial:**
    ![Página Inicial](URL_DA_IMAGEM_HOME_AQUI)
* **Detalhes do Artista:**
    ![Detalhes do Artista](URL_DA_IMAGEM_ARTISTA_AQUI)
* **Player da Música:**
    ![Player da Música](URL_DA_IMAGEM_PLAYER_AQUI)

---

## 🤝 Contribuindo

Contribuições são o que tornam a comunidade open source um lugar incrível para aprender, inspirar e criar. Qualquer contribuição que você fizer será **muito apreciada**.

Se você tiver uma sugestão para melhorar este projeto, por favor, faça um fork do repositório e crie um pull request. Você também pode simplesmente abrir uma issue com a tag "enhancement".
Não se esqueça de dar uma estrela ao projeto! Obrigado novamente!

1.  Faça um Fork do projeto
2.  Crie sua Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4.  Push para a Branch (`git push origin feature/AmazingFeature`)
5.  Abra um Pull Request

---

## 📄 Licença

Distribuído sob a Licença MIT. Veja `LICENSE.txt` para mais informações.
---

## 🧑‍💻 Autor
* **Victor Harnisch / Estudo** - https://github.com/VictorHarnnisch - harnisch.victor@gmail.com


---

<p align="center">
  Feito com ❤️ por Vitinho_Deutsch
</p>
