<h1 align='center'>🚧 PROJECT_NAME_HERE in progress... 🚧</h1>

<div align='center'>

  ![project-img](https://www.breatheazy.co.uk/wp-content/uploads/2023/09/Untitled-design-35-1080x675.png)
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)

  [🎨 Design](link-to-Figma)

  [🇵🇹 Português](./docs/README-pt.md)

</div>

## 📚 Summary
- [❕ About](#about)
- [📖 Instructions](#instructions)
  - [📥 Install](#install)
  - [🚀 Run Locally](#locally)
  - [📋 Run Unit Tests](#unit-tests)
  - [🏁 Run End-To-End Tests](#e2e-tests)
  - [📔 Run Storybook](#storybook)
- [⚡ Endpoints](#endpoints)
- [📂 Structure](#structure)
- [🧰 Technologies](#technologies)
- [📸 Screenshots and 🎥 Recordings](#screenshots-prints)
- [👤 Author](#author)
- [📄 License](#license)

### <a id='about' style='text-decoration: none; color: inherit;'>❕ About</a>
Describe well the project here, comment where the idea came, its objective, its functionalities, some prints showing them in the order of the most common flow of the application

### <a id='instructions' style='text-decoration: none; color: inherit;'>📖 Instructions</a>
#### <a id='instalar' style='text-decoration: none; color: inherit;'>📥 Install</a>
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

#### <a id='locally' style='text-decoration: none; color: inherit;'>🚀 Run Locally</a>
Paste the command into a terminal, the application will be accessable through this [link](http://localhost:5173)
```sh
npm run dev
```

#### <a id='unit-tests' style='text-decoration: none; color: inherit;'>📋 Run Unit Tests</a>
Paste the command into a terminal, they will be exectued one after the other mentioning if there were failed tests
```sh
npm run tests
```

#### <a id='e2e-tests' style='text-decoration: none; color: inherit;'>🏁 Run End-To-End Tests</a>
Paste the command into a terminal, the tests will be open in a browser tab automatically, controlling it like an actual user, clicking on buttons, interacting with forms, etc... The results will appear within the own interface
```sh
npm run tests-e2e
```

#### <a id='storybook' style='text-decoration: none; color: inherit;'>📔 Run Storybook</a>
Paste the command into a terminal, the project's components documentation will be accessible through this [link](http://localhost:6006)
```sh
npm run storybook
```

### <a id='endpoints' style='text-decoration: none; color: inherit;'>⚡ Endpoints</a>
In order to make requests to the server with 🥧 HTTPie directly from the terminal, you would have to follow its CLI [installation guide](https://httpie.io/docs/cli/main-features)
#### POST endpoint title
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

#### GET endpoint title
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

#### PUT endpoint title
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

#### DELETE endpoint title
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

#### PATCH endpoint title
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

#### Non existing route
When trying to access a route that doesn't exists in the server

Response
```
HTTP/1.1 404 Not Found
Connection: keep-alive
Content-type: application/json

"Route not found"
```

### <a id='structure' style='text-decoration: none; color: inherit;'>📂 Structure</a>
```
│ .storybook/
│   └── ...
│ .tests/
│   └── ...
│ src/
│   ├── assets/
│   │     └── ...
│   ├── components/
│   │     ├── component x/
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

### <a id='technologies' style='text-decoration: none; color: inherit;'>🧰 Technologies</a>
#### Build Tools
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)

#### Components
[![Font Awesome](https://img.shields.io/badge/Font_Awesome-339AF0?style=for-the-badge&logo=font-awesome&logoColor=white)](https://fontawesome.com/)
[![Lucide React](https://img.shields.io/badge/Lucide-2C3E50?style=for-the-badge&logo=lucide&logoColor=white)](https://lucide.dev/)
[![Phosphor Icons](https://img.shields.io/badge/Phosphor%20Icons-c4e456?style=for-the-badge&logo=phosphoricons&logoColor=black)](https://phosphoricons.com/)
[![Radix UI](https://img.shields.io/badge/Radix_UI-29ABE2?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://radix-ui.com/)
[![React Loading Skeleton](https://img.shields.io/badge/React%20Loading%20Skeleton-333?style=for-the-badge&logo=react&logoColor=white)](https://www.npmjs.com/package/react-loading-skeleton)
[![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?style=for-the-badge&logo=react&logoColor=white)](https://shadcn.dev)
[![Styled-Components](https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white)](https://styled-components.com/)
[![Toastify](https://img.shields.io/badge/Toastify-FF5733?style=for-the-badge&logo=react&logoColor=white)](https://fkhadra.github.io/react-toastify/introduction)

#### Documentation
[![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white)](https://storybook.js.org/)
[![MSW](https://img.shields.io/badge/MSW-ff6a33?style=for-the-badge&logo=msw&logoColor=white)](https://mswjs.io/)

#### Back-end Framework
[![Fastify](https://img.shields.io/badge/fastify-000000?style=for-the-badge&logo=fastify&logoColor=white)](https://www.fastify.io/)

#### Front-end Framework
[![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React.js](https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![React Router DOM](https://img.shields.io/badge/React%20Router%20DOM-61DAFB?style=for-the-badge&logo=react-router&logoColor=white&color=red)](https://reactrouter.com/en/main)
[![React Query](https://img.shields.io/badge/React_Query-FF4154?style=for-the-badge&logo=react-query&logoColor=white)](https://tanstack.com/query/v3)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

#### Database
[![Knex](https://img.shields.io/badge/knex-ff5722?style=for-the-badge&logo=knex&logoColor=white)](https://knexjs.org/)
[![SQLite](https://img.shields.io/badge/sqlite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)

#### Styling
[![PostCSS](https://img.shields.io/badge/PostCSS-DD3A0A?style=for-the-badge&logo=postcss&logoColor=white)](https://postcss.org/)
[![Tailwind CSS](https://img.shields.io/badge/tailwind--css-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)

#### Testing
[![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)](https://playwright.dev/)
[![React Testing Library](https://img.shields.io/badge/React%20Testing%20Library-E33332?style=for-the-badge&logo=testing-library&logoColor=white)](https://testing-library.com/docs/react-testing-library/intro)
[![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)](https://jestjs.io/)
[![Vitest](https://img.shields.io/badge/vitest-506E10?style=for-the-badge&logo=vitest&logoColor=FCC72B)](https://vitest.dev/)
[![MSW](https://img.shields.io/badge/MSW-ff6a33?style=for-the-badge&logo=msw&logoColor=white)](https://mswjs.io/)

#### Utilities
[![date-fns](https://img.shields.io/badge/date--fns-770c56?style=for-the-badge&logo=date-fns&logoColor=white)](https://date-fns.org/)
[![Day.js](https://img.shields.io/badge/Day.js-FF6F00?style=for-the-badge&logo=dayjs&logoColor=white)](https://day.js.org/)
[![dotenv](https://img.shields.io/badge/dotenv-ECD53F?style=for-the-badge&logo=.env&logoColor=black)](https://github.com/motdotla/dotenv)
[![ESLint](https://img.shields.io/badge/eslint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)](https://eslint.org/)
[![React Day Picker](https://img.shields.io/badge/React%20Day%20Picker-42A5F5?style=for-the-badge&logo=react&logoColor=white)](https://react-day-picker.js.org/)
[![React Hook Form](https://img.shields.io/badge/React_Hook_Form-FF6B6B?style=for-the-badge&logo=react&logoColor=white)](https://react-hook-form.com/)
[![TSX](https://img.shields.io/badge/tsx-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.npmjs.com/package/tsx)
[![Zod](https://img.shields.io/badge/Zod-007ACC?style=for-the-badge&logo=superman&logoColor=white)](https://zod.dev/)

### <a id='screenshots-prints' style='text-decoration: none; color: inherit;'>📸 Screenshots and 🎥 Recordings</a>
For a longer video demonstration click here and like my post on <a href='link-to-project-post-on-linkedin'>LinkedIn</a>

![example-screenshot](https://as2.ftcdn.net/v2/jpg/02/66/72/41/1000_F_266724172_Iy8gdKgMa7XmrhYYxLCxyhx6J7070Pr8.jpg)
<p align='center'>A very short description of what is happening in the image</p>

### <a id='author' style='text-decoration: none; color: inherit;'>👤 Author</a>
<div style='display: flex; align-items: center;'>
		<img src='https://github.com/mar-alv.png' alt='Marcelo Alvarez GitHub profile picture' style='width: 150px; border-radius: 50%; margin-right: 20px;'>
		<div>
				<strong>Marcelo Alvarez</strong>
				<br>
				<em>Front-end Developer</em><br>
				<span>"Some AI generated funny quote here 😗"</span><br>
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

### <a id='license' style='text-decoration: none; color: inherit;'>📄 License</a>
Licensed under [MIT](./LICENSE)
