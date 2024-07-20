<h1 align='center'>🚧 PROJECT_NAME_HERE in progress... 🚧</h1>

<div align='center'>

  ![project-img](https://www.breatheazy.co.uk/wp-content/uploads/2023/09/Untitled-design-35-1080x675.png)
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)

  [🎨 Design](link-to-Figma)

  [🇬🇧 English](#en) / [🇧🇷 Português](#pt-br)

</div>

## <a id='en' style='text-decoration: none; color: inherit;'>🇬🇧 English</a>

### 📚 Summary
- [❕ About](#en-about)
- [📖 Instructions](#en-instructions)
  - [📥 Install](#en-install)
  - [🚀 Run Locally](#en-locally)
  - [📋 Run Unit Tests](#en-unit-tests)
  - [🏁 Run End-To-End Tests](#en-e2e-tests)
  - [📔 Run Storybook](#en-storybook)
- [⚡ Endpoints](#en-endpoints)
- [📂 Structure](#en-structure)

#### <a id='en-about' style='text-decoration: none; color: inherit;'>❕ About</a>
Describe well the project here, comment where the idea came, its objective, its functionalities, some prints showing them in the order of the most common flow of the application

#### <a id='en-instructions' style='text-decoration: none; color: inherit;'>📖 Instructions</a>
##### <a id='en-instalar' style='text-decoration: none; color: inherit;'>📥 Install</a>
Paste this 1º command into a terminal opened within a folder of your preference to clone the project
```sh
git clone https://github.com/mar-alv/REPO.git
```

Then run one of the versions of the 2º command to install the dependencies
```sh
npm i
```
```sh
npm install
```

##### <a id='en-locally' style='text-decoration: none; color: inherit;'>🚀 Run Locally</a>
Paste the command into a terminal, the application will be accessable through this [link](http://localhost:5173)
```sh
npm run dev
```

##### <a id='en-unit-tests' style='text-decoration: none; color: inherit;'>📋 Run Unit Tests</a>
Paste the command into a terminal, they will be exectued one after the other mentioning if there were failed tests
```sh
npm run tests
```

##### <a id='en-e2e-tests' style='text-decoration: none; color: inherit;'>🏁 Run End-To-End Tests</a>
Paste the command into a terminal, the tests will be open in a browser tab automatically, controlling it like an actual user, clicking on buttons, interacting with forms, etc... The results will appear within the own interface
```sh
npm run tests-e2e
```

##### <a id='en-storybook' style='text-decoration: none; color: inherit;'>📔 Run Storybook</a>
Paste the command into a terminal, the project's components documentation will be accessible through this [link](http://localhost:6006)
```sh
npm run storybook
```

#### <a id='en-endpoints' style='text-decoration: none; color: inherit;'>⚡ Endpoints</a>
In order to make requests to the server with 🥧 HTTPie directly from the terminal, you would have to follow its CLI [installation guide](https://httpie.io/docs/cli/main-features)
##### POST endpoint title
POST endpoint description of what it does
```sh
curl -X POST http://localhost:3001/route -h "Content-Type: application/json" -d '{"request_body":"here"}'
```

With 🥧 HTTPie
```sh
http POST http://localhost:3001/route < httpie/post.json
```

Responses
```
# When successfully doing it

HTTP/1.1 201 Created
Connection: keep-alive
Content-type: application/json

# When not providing a valid request body

HTTP/1.1 400 Bad Request
Content-type: application/json
```

##### GET endpoint title
GET endpoint description of what it does
```sh
curl -X GET 'http://localhost:3001/route' -h "Content-Type: application/json"
```
```sh
curl -X GET 'http://localhost:3001/route?query_parameter=here' -h "Content-Type: application/json"
```

With 🥧 HTTPie
```sh
http GET http://localhost:3001/route
```
```sh
http GET http://localhost:3001/route?query_parameter=here
```

Responses
```
# When successfully doing it

HTTP/1.1 200 OK
Connection: keep-alive
Content-type: application/json

{
	...
}

# Nothing found

HTTP/1.1 200 OK
Connection: keep-alive
Content-type: application/json

{}
```

##### PUT endpoint title
PUT endpoint description of what it does
```sh
curl -X PUT http://localhost:3001/route/123- -h "Content-Type: application/json" -d '{"request_body":"here"}'
```

With 🥧 HTTPie
```sh
http PUT http://localhost:3001/tasks/123 < httpie/put.json
```

Responses
```
# When successfully doing it

HTTP/1.1 204 No Content
Connection: keep-alive
Content-type: application/json

# When not providing a valid request body

HTTP/1.1 400 Bad Request
Connection: keep-alive
Content-type: application/json

# When not finding it by the id

HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json
```

##### DELETE endpoint title
DELETE endpoint description of what it does
```sh
curl -X DELETE http://localhost:3001/route/123 -h "Content-Type: application/json"
```

With 🥧 HTTPie
```sh
http DELETE http://localhost:3001/tasks/123
```

Responses
```
# When successfully doing it

HTTP/1.1 204 No Content
Connection: keep-alive
Content-type: application/json

# When not finding it by the id

HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json
```

##### PATCH endpoint title
PATCH endpoint description of what it does
```sh
curl -X PATCH http://localhost:3001/route/123/something -h "Content-Type: application/json"
```

With 🥧 HTTPie
```sh
http PATCH http://localhost:3001/route/123/something
```

Responses
```
# When successfully doing it

HTTP/1.1 204 No Content
Connection: keep-alive
Content-type: application/json

# When not finding it by the id

HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json
```

##### Non existing route
When trying to access a route that doesn't exists in the server

Response
```
HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json

"Route not found"
```

#### <a id='en-structure' style='text-decoration: none; color: inherit;'>📂 Structure</a>
```
│ .storybook/
│   └── ... files to keep Storybook working
│ .tests/
│   └── ... files to keep tests working
│ src/
│   ├── assets/
│   │     └── ... svgs used
│   ├── components/
│   │     ├── componente x/
│   │     │     ├── index.tsx
│   │     │     └── styles.ts
│   │     └── ...
│   ├── contexts/
│   │     └── ... contexts and providers
│   ├── styles/
│   │     └── ... global styles and default theme
│   ├── interfaces/
│   │     └── ... interfaces used
│   └── ...
│ stories/
│   ├── components/
│   │     └── ... stories of the components
│   ├── ... generic stories (color, icons e typography)
│   └── ... stories-utils.tsx // util functions for stories
│ tests/
│   ├── ... unit tests
│   └── ... tests-utils.tsx // util functions for tests
```

## <a id='pt-br' style='text-decoration: none; color: inherit;'>🇧🇷 Português</a>

### 📚 Sumário
- [❕ Sobre](#pt-br-sobre)
- [📖 Instruções](#pt-br-instrucoes)
  - [📥 Instalar](#pt-br-instalar)
  - [🚀 Rodar Localmente](#pt-br-localmente)
  - [📋 Rodar Testes Unitários](#pt-br-testes-unitarios)
  - [🏁 Rodar Testes End-To-End](#pt-br-testes-e2e)
  - [📔 Rodar Storybook](#pt-br-storybook)
- [⚡ Endpoints](#pt-br-endpoints)
- [📂 Estrutura](#pt-br-estrutura)

#### <a id='pt-br-sobre' style='text-decoration: none; color: inherit;'>❕ Sobre</a>
Descreva bem o projeto aqui, comente de onde veio a ideia, qual sua finalidade, qual suas funcionalidades, alguns prints mostrando elas na ordem do fluxo mais comum da aplicação

#### <a id='pt-br-instrucoes' style='text-decoration: none; color: inherit;'>📖 Instruções</a>
##### <a id='pt-br-instalar' style='text-decoration: none; color: inherit;'>📥 Instalar</a>
Cole o 1º comando em um terminal aberto dentro da pasta de sua preferência para clonar o projeto
```sh
git clone https://github.com/mar-alv/REPO.git
```

Em seguida rode uma das versões do 2º comando para instalar as dependências
```sh
npm i
```
```sh
npm install
```

##### <a id='pt-br-localmente' style='text-decoration: none; color: inherit;'>🚀 Rodar Localmente</a>
Cole o comando em um terminal, a aplicação estará acessível através desse [link](http://localhost:5173)
```sh
npm run dev
```

##### <a id='pt-br-testes-unitarios' style='text-decoration: none; color: inherit;'>📋 Rodar Testes Unitários</a>
Cole o comando em um terminal, eles serão executados um após o outro apontando se houve testes falhos
```sh
npm run tests
```

##### <a id='pt-br-testes-e2e' style='text-decoration: none; color: inherit;'>🏁 Rodar Testes End-To-End</a>
Cole o comando num terminal, os testes serão abertos numa aba do navegador automaticamente, controlando ela como um usuário real, clicando em botões, interagindo com formulários, etc... Os resultados aparecerão na própria interface
```sh
npm run tests-e2e
```

##### <a id='pt-br-storybook' style='text-decoration: none; color: inherit;'>📔 Rodar Storybook</a>
Cole o comando num terminal, a documentação dos componentes do projeto estará acessível através desse [link](http://localhost:6006)
```sh
npm run storybook
```

##### <a id='pt-br-endpoints' style='text-decoration: none; color: inherit;'>⚡ Endpoints</a>
Para fazer requisições ao servidor com 🥧 HTTPie diretamente do terminal, é necessário seguir o [guia de instalação](https://httpie.io/docs/cli/main-features) da CLI
##### Título do endpoint POST
Descrição do que o endpoint POST faz
```sh
curl -X POST http://localhost:3001/rota -h "Content-Type: application/json" -d '{"corpo_da_requisicao":"aqui"}'
```

Com 🥧 HTTPie
```sh
http POST http://localhost:3001/rota < httpie/post.json
```

Respostas
```
# Ao fazer isso com sucesso

HTTP/1.1 201 Created
Connection: keep-alive
Content-type: application/json

# Ao enviar um corpo de requisição inválido

HTTP/1.1 400 Bad Request
Content-type: application/json
```

##### Título do endpoint GET
Descrição do que o endpoint GET faz
```sh
curl -X GET 'http://localhost:3001/rota' -h "Content-Type: application/json"
```
```sh
curl -X GET 'http://localhost:3001/rota?parametro=aqui' -h "Content-Type: application/json"
```

Com 🥧 HTTPie
```sh
http GET http://localhost:3001/rota
```
```sh
http GET http://localhost:3001/rota?parametro=aqui
```

Respostas
```
# Ao fazer isso com sucesso

HTTP/1.1 200 OK
Connection: keep-alive
Content-type: application/json

{
	...
}

# Não encontrando nada

HTTP/1.1 200 OK
Connection: keep-alive
Content-type: application/json

{}
```

##### Título do endpoint PUT
Descrição do que o endpoint PUT faz
```sh
curl -X PUT http://localhost:3001/rota/123- -h "Content-Type: application/json" -d '{"corpo_da_requisicao":"aqui"}'
```

Com 🥧 HTTPie
```sh
http PUT http://localhost:3001/rota/123 < httpie/put.json
```

Respostas
```
# Ao fazer isso com sucesso

HTTP/1.1 204 No Content
Connection: keep-alive
Content-type: application/json

# Ao enviar um corpo de requisição inválido

HTTP/1.1 400 Bad Request
Connection: keep-alive
Content-type: application/json

# Ao não encontrar isso pelo seu id

HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json
```

##### Título do endpoint DELETE
Descrição do que o endpoint DELETE faz
```sh
curl -X DELETE http://localhost:3001/rota/123 -h "Content-Type: application/json"
```

Com 🥧 HTTPie
```sh
http DELETE http://localhost:3001/rota/123
```

Respostas
```
# Ao fazer isso com sucesso

HTTP/1.1 204 No Content
Connection: keep-alive
Content-type: application/json

# Ao não encontrar isso pelo seu id

HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json
```

##### Título do endpoint PATCH
Descrição do que o endpoint PATCH faz
```sh
curl -X PATCH http://localhost:3001/rota/123/algo -h "Content-Type: application/json"
```

Com 🥧 HTTPie
```sh
http PATCH http://localhost:3001/rota/123/algo
```

Respostas
```
# Ao fazer isso com sucesso

HTTP/1.1 204 No Content
Connection: keep-alive
Content-type: application/json

# Ao não encontrar isso pelo seu id

HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json
```

##### Rota não existente
Ao tentar acessar uma rota que não existe no servidor

Resposta
```
HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json

"Route not found"
```

#### <a id='pt-br-estrutura' style='text-decoration: none; color: inherit;'>📂 Estrutura</a>
```
│ .storybook/
│   └── ... arquivos que mantém o funcionamento do Storybook
│ .tests/
│   └── ... arquivos que mantém o funcionamento dos testes
│ src/
│   ├── assets/
│   │     └── ... svgs usados
│   ├── components/
│   │     ├── componente x/
│   │     │     ├── index.tsx
│   │     │     └── styles.ts
│   │     └── ...
│   ├── contexts/
│   │     └── ... contextos e providers
│   ├── styles/
│   │     └── ... estilos globais e default
│   ├── interfaces/
│   │     └── ... interfaces usadas
│   └── ...
│ stories/
│   ├── components/
│   │     └── ... stories dos componentes
│   ├── ... stories genéricos(cor, ícones e tipografia)
│   └── ... stories-utils.tsx // funções utilitárias pros stories
│ tests/
│   ├── ... testes unitários
│   └── ... tests-utils.tsx // funções utilitárias pros testes
```

## 🧰 Technologies
### Build Tools
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)

### Documentation
[![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white)](https://storybook.js.org/)

### Components
[![Radix UI](https://img.shields.io/badge/Radix_UI-29ABE2?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://radix-ui.com/)

### Back-end Framework
[![Fastify](https://img.shields.io/badge/fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)](https://www.fastify.io/)

### Front-end Framework
[![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React.js](https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![React Router DOM](https://img.shields.io/badge/React%20Router%20DOM-61DAFB?style=for-the-badge&logo=react-router&logoColor=white&color=red)](https://reactrouter.com/en/main)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

### Database
[![Knex](https://img.shields.io/badge/knex-ff5722?style=for-the-badge&logo=knex&logoColor=white)](https://knexjs.org/)
[![SQLite](https://img.shields.io/badge/sqlite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)

### Styling
[![Font Awesome](https://img.shields.io/badge/Font_Awesome-339AF0?style=for-the-badge&logo=font-awesome&logoColor=white)](https://fontawesome.com/)
[![Phosphor Icons](https://img.shields.io/badge/Phosphor%20Icons-c4e456?style=for-the-badge&logo=phosphoricons&logoColor=black)](https://phosphoricons.com/)
[![Styled-Components](https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white)](https://styled-components.com/)

### Testing
[![React Testing Library](https://img.shields.io/badge/React%20Testing%20Library-E33332?style=for-the-badge&logo=testing-library&logoColor=white)](https://testing-library.com/docs/react-testing-library/intro)
[![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)](https://jestjs.io/)
[![Vitest](https://img.shields.io/badge/vitest-506E10?style=for-the-badge&logo=vitest&logoColor=FCC72B)](https://vitest.dev/)

### Utilities
[![dotenv](https://img.shields.io/badge/dotenv-ECD53F?style=for-the-badge&logo=.env&logoColor=black)](https://github.com/motdotla/dotenv)
[![ESLint](https://img.shields.io/badge/eslint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)](https://eslint.org/)
[![React Hook Form](https://img.shields.io/badge/React_Hook_Form-FF6B6B?style=for-the-badge&logo=react&logoColor=white)](https://react-hook-form.com/)
[![TSX](https://img.shields.io/badge/tsx-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.npmjs.com/package/tsx)
[![Zod](https://img.shields.io/badge/Zod-007ACC?style=for-the-badge&logo=superman&logoColor=white)](https://zod.dev/)

## 📸 Screenshots and 🎥 Recordings
For a longer video demonstration click here and like my post on
<a href='link-to-project-post-on-linkedin'>LinkedIn</a>

![example-screenshot](https://as2.ftcdn.net/v2/jpg/02/66/72/41/1000_F_266724172_Iy8gdKgMa7XmrhYYxLCxyhx6J7070Pr8.jpg)
A very short description of what is happening in the image

## Author
<div style='display: flex; align-items: center;'>
    <img src='https://github.com/mar-alv.png' alt='Marcelo Alvarez GitHub profile picture' style='width: 150px; border-radius: 50%; margin-right: 20px;'>
    <div>
        <strong>Marcelo Alvarez</strong>
        <br>
        <em>Front-end Developer</em><br>
        <span>"Some AI generated funny quote here 😗"</span><br>
        <a href='https://www.linkedin.com/in/marcelo-dos-santos-alvarez-474406180/'>LinkedIn</a> |
        <a href='/'>Portfolio</a>
    </div>
</div>

## License
Licensed under [MIT](./LICENSE)
