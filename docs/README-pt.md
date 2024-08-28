<h1 align='center'>🚧 NOME_DO_PROJETO_AQUI em progresso... 🚧</h1>

<div align='center'>

  ![project-img](https://www.breatheazy.co.uk/wp-content/uploads/2023/09/Untitled-design-35-1080x675.png)
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)

  [🎨 Design](link-to-Figma)

  [⬅️ Voltar](../README.md)

</div>

## 📚 Sumário
- [❕ Sobre](#about)
- [📖 Instruções](#instructions)
  - [📥 Instalar](#install)
  - [🚀 Rodar Localmente](#locally)
  - [📋 Rodar Testes Unitários](#unit-tests)
  - [🏁 Rodar Testes End-To-End](#e2e-tests)
  - [📔 Rodar Storybook](#storybook)
- [⚡ Endpoints](#endpoints)
- [📂 Estrutura](#structure)
- [🧰 Tecnologias](#technologies)
- [📸 Prints e 🎥 Gravações](#screenshots-prints)
- [👤 Autor](#author)
- [📄 Licença](#license)

### <a id='about' style='text-decoration: none; color: inherit;'>❕ Sobre</a>
Descreva bem o projeto aqui, comente de onde veio a ideia, qual sua finalidade, qual suas funcionalidades, alguns prints mostrando elas na ordem do fluxo mais comum da aplicação

### <a id='instructions' style='text-decoration: none; color: inherit;'>📖 Instruções</a>
#### <a id='install' style='text-decoration: none; color: inherit;'>📥 Instalar</a>
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

#### <a id='locally' style='text-decoration: none; color: inherit;'>🚀 Rodar Localmente</a>
Cole o comando em um terminal, a aplicação estará acessível através desse [link](http://localhost:5173)
```sh
npm run dev
```

#### <a id='unit-tests' style='text-decoration: none; color: inherit;'>📋 Rodar Testes Unitários</a>
Cole o comando em um terminal, eles serão executados um após o outro apontando se houve testes falhos
```sh
npm run tests
```

#### <a id='e2e-tests' style='text-decoration: none; color: inherit;'>🏁 Rodar Testes End-To-End</a>
Cole o comando num terminal, os testes serão abertos numa aba do navegador automaticamente, controlando ela como um usuário real, clicando em botões, interagindo com formulários, etc... Os resultados aparecerão na própria interface
```sh
npm run tests-e2e
```

#### <a id='storybook' style='text-decoration: none; color: inherit;'>📔 Rodar Storybook</a>
Cole o comando num terminal, a documentação dos componentes do projeto estará acessível através desse [link](http://localhost:6006)
```sh
npm run storybook
```

#### <a id='endpoints' style='text-decoration: none; color: inherit;'>⚡ Endpoints</a>
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

#### <a id='structure' style='text-decoration: none; color: inherit;'>📂 Estrutura</a>
```
│ .storybook/
│   └── ...
│ .tests/
│   └── ...
│ src/
│   ├── assets/
│   │     └── ...
│   ├── components/
│   │     ├── componente x/
│   │     │     ├── index.tsx
│   │     │     └── styles.ts
│   │     └── ...
│   ├── contexts/
│   │     └── ...
│   ├── styles/
│   │     └── ...
│   ├── interfaces/
│   │     └── ...
│   └── ...
│ stories/
│   ├── components/
│   │     └── ...
│   └── ...
│ tests/
│   └── ...
```

## <a id='technologies' style='text-decoration: none; color: inherit;'>🧰 Tecnologias</a>
### Build
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)

### Componentes
[![Font Awesome](https://img.shields.io/badge/Font_Awesome-339AF0?style=for-the-badge&logo=font-awesome&logoColor=white)](https://fontawesome.com/)
[![Lucide React](https://img.shields.io/badge/Lucide-2C3E50?style=for-the-badge&logo=lucide&logoColor=white)](https://lucide.dev/)
[![Phosphor Icons](https://img.shields.io/badge/Phosphor%20Icons-c4e456?style=for-the-badge&logo=phosphoricons&logoColor=black)](https://phosphoricons.com/)
[![Radix UI](https://img.shields.io/badge/Radix_UI-29ABE2?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://radix-ui.com/)
[![React Loading Skeleton](https://img.shields.io/badge/React%20Loading%20Skeleton-333?style=for-the-badge&logo=react&logoColor=white)](https://www.npmjs.com/package/react-loading-skeleton)
[![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?style=for-the-badge&logo=react&logoColor=white)](https://shadcn.dev)
[![Styled-Components](https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white)](https://styled-components.com/)
[![Toastify](https://img.shields.io/badge/Toastify-FF5733?style=for-the-badge&logo=react&logoColor=white)](https://fkhadra.github.io/react-toastify/introduction)

### Documentação
[![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white)](https://storybook.js.org/)
[![MSW](https://img.shields.io/badge/MSW-ff6a33?style=for-the-badge&logo=msw&logoColor=white)](https://mswjs.io/)

### Framework Back-end
[![Fastify](https://img.shields.io/badge/fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)](https://www.fastify.io/)

### Framework Front-end
[![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React.js](https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![React Router DOM](https://img.shields.io/badge/React%20Router%20DOM-61DAFB?style=for-the-badge&logo=react-router&logoColor=white&color=red)](https://reactrouter.com/en/main)
[![React Query](https://img.shields.io/badge/React_Query-FF4154?style=for-the-badge&logo=react-query&logoColor=white)](https://tanstack.com/query/v3)
[![TypeScript](https://img.shields.io/badge/TypeScri3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

### Banco de Dados
[![Knex](https://img.shields.io/badge/knex-ff5722?style=for-the-badge&logo=knex&logoColor=white)](https://knexjs.org/)
[![SQLite](https://img.shields.io/badge/sqlite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)

### Estilização
[![PostCSS](https://img.shields.io/badge/PostCSS-DD3A0A?style=for-the-badge&logo=postcss&logoColor=white)](https://postcss.org/)
[![Tailwind CSS](https://img.shields.io/badge/tailwind--css-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

### Testes
[![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)](https://playwright.dev/)
[![React Testing Library](https://img.shields.io/badge/React%20Testing%20Library-E33332?style=for-the-badge&logo=testing-library&logoColor=white)](https://testing-library.com/docs/react-testing-library/intro)
[![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)](https://jestjs.io/)
[![Vitest](https://img.shields.io/badge/vitest-506E10?style=for-the-badge&logo=vitest&logoColor=FCC72B)](https://vitest.dev/)
[![MSW](https://img.shields.io/badge/MSW-ff6a33?style=for-the-badge&logo=msw&logoColor=white)](https://mswjs.io/)

### Utilidades
[![date-fns](https://img.shields.io/badge/date--fns-770c56?style=for-the-badge&logo=date-fns&logoColor=white)](https://date-fns.org/)
[![Day.js](https://img.shields.io/badge/Day.js-FF6F00?style=for-the-badge&logo=dayjs&logoColor=white)](https://day.js.org/)
[![dotenv](https://img.shields.io/badge/dotenv-ECD53F?style=for-the-badge&logo=.env&logoColor=black)](https://github.com/motdotla/dotenv)
[![ESLint](https://img.shields.io/badge/eslint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)](https://eslint.org/)
[![React Day Picker](https://img.shields.io/badge/React%20Day%20Picker-42A5F5?style=for-the-badge&logo=react&logoColor=white)](https://react-day-picker.js.org/)
[![React Hook Form](https://img.shields.io/badge/React_Hook_Form-FF6B6B?style=for-the-badge&logo=react&logoColor=white)](https://react-hook-form.com/)
[![TSX](https://img.shields.io/badge/tsx-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.npmjs.com/package/tsx)
[![Zod](https://img.shields.io/badge/Zod-007ACC?style=for-the-badge&logo=superman&logoColor=white)](https://zod.dev/)

## <a id='screenshots-prints' style='text-decoration: none; color: inherit;'>📸 Prints e 🎥 Gravações</a>
Para uma demonstração mais longa clique aqui e curta meu post no
<a href='link-to-project-post-on-linkedin'>LinkedIn</a>

![example-screenshot](https://as2.ftcdn.net/v2/jpg/02/66/72/41/1000_F_266724172_Iy8gdKgMa7XmrhYYxLCxyhx6J7070Pr8.jpg)
<p align='center'>Um descrição muito breve do que está acontecendo na imagem</p>

## <a id='author' style='text-decoration: none; color: inherit;'>👤 Autor</a>
<div style='display: flex; align-items: center;'>
		<img src='https://github.com/mar-alv.png' alt='Marcelo Alvarez GitHub profile picture' style='width: 150px; border-radius: 50%; margin-right: 20px;'>
		<div>
				<strong>Marcelo Alvarez</strong>
				<br>
				<em>Front-end Developer</em><br>
				<span>"Uma citação engraçada gerada por IA aqui 😗"</span><br>
				<a href='https://www.linkedin.com/in/mar-alv'>
					<img
						alt='LinkedIn'
						src='https://img.shields.io/badge/LinkedIn-Marcelo%20Alvarez-0077B5?logo=linkedin&logoColor=white'
					/>
				</a>
				<a href='https://mar-alv.github.io/'>
					<img
						alt='Portfolio'
						src='https://img.shields.io/badge/Portfolio-Marcelo%20Alvarez-000?style=flat&logo=portfolio&logoColor=white'
					/>
				</a>
		</div>
</div>

## <a id='license' style='text-decoration: none; color: inherit;'>📄 Licença</a>
Licenciado via [MIT](./LICENSE)
