<h1 align='center'>🚧 PROJECT_NAME_HERE in progress... 🚧</h1>

<div align='center'>

  ![project-img](https://www.breatheazy.co.uk/wp-content/uploads/2023/09/Untitled-design-35-1080x675.png)
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)

  [🎨 Design](link-to-Figma)

  [🇧🇷 Português](#pt-br) / [🇬🇧 English](#en)

</div>

## <a id='pt-br' style='text-decoration: none; color: inherit;'>🇧🇷 Português</a>

### 📚 Sumário
- [❕ Sobre](#pt-br-sobre)
- [📖 Instruções](#pt-br-instrucoes)
  - [📥 Instalar](#pt-br-instalar)
  - [🚀 Rodar Localmente](#pt-br-localmente)
  - [📋 Rodar Testes Unitários](#pt-br-testes-unitarios)
  - [🏁 Rodar Testes End-To-End](#pt-br-testes-e2e)
  - [📔 Rodar Storybook](#pt-br-storybook)
- [📂 Estrutura](#pt-br-estrutura)

#### <a id='pt-br-sobre' style='text-decoration: none; color: inherit;'>❕ Sobre</a>
Descreva bem o projeto aqui, comente de onde veio a ideia, qual sua finalidade, qual suas funcionalidades, alguns prints mostrando elas na ordem do fluxo mais comum da aplicação

#### <a id='pt-br-instrucoes' style='text-decoration: none; color: inherit;'>📖 Instruções</a>
##### <a id='pt-br-instalar' style='text-decoration: none; color: inherit;'>📥 Instalar</a>
Cole o 1º comando em um terminal aberto dentro da pasta de sua preferência para clonar o projeto, em seguida rode uma das versões do 2º comando para instalar as dependências
```sh
git clone https://github.com/mar-alv/REPO.git
npm i # Ou npm install
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

## <a id='en' style='text-decoration: none; color: inherit;'>🇬🇧 English</a>

### 📚 Summary
- [❕ About](#en-about)
- [📖 Instructions](#en-instructions)
  - [📥 Install](#en-install)
  - [🚀 Run Locally](#en-locally)
  - [📋 Run Unit Tests](#en-unit-tests)
  - [🏁 Run End-To-End Tests](#en-e2e-tests)
  - [📔 Run Storybook](#en-storybook)
- [📂 Structure](#en-structure)

#### <a id='en-about' style='text-decoration: none; color: inherit;'>❕ About</a>
Describe well the project here, comment where the idea came, its objective, its functionalities, some prints showing them in the order of the most common flow of the application

#### <a id='en-instructions' style='text-decoration: none; color: inherit;'>📖 Instructions</a>
##### <a id='en-instalar' style='text-decoration: none; color: inherit;'>📥 Install</a>
Paste the 1º command into a terminal opened within a folder of your preference to clone the project, then run one of the versions of the 2º command to install the dependencies
```sh
git clone https://github.com/mar-alv/REPO.git
npm i # Or npm install
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

## 🧰 Technologies
### Build Tools
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)

### Documentation
[![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=for-the-badge&logo=storybook&logoColor=white)](https://storybook.js.org/)

### Components
[![Radix UI](https://img.shields.io/badge/Radix_UI-29ABE2?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://radix-ui.com/)

### Front-end Framework
[![NextJS](https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)](https://nextjs.org/)
[![React.js](https://img.shields.io/badge/React.js-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![React Router DOM](https://img.shields.io/badge/React%20Router%20DOM-61DAFB?style=for-the-badge&logo=react-router&logoColor=white&color=red)](https://reactrouter.com/en/main)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

### Styling
[![Font Awesome](https://img.shields.io/badge/Font_Awesome-339AF0?style=for-the-badge&logo=font-awesome&logoColor=white)](https://fontawesome.com/)
[![Phosphor Icons](https://img.shields.io/badge/Phosphor%20Icons-c4e456?style=for-the-badge&logo=phosphoricons&logoColor=black)](https://phosphoricons.com/)
[![Styled-Components](https://img.shields.io/badge/styled--components-DB7093?style=for-the-badge&logo=styled-components&logoColor=white)](https://styled-components.com/)

### Testing
[![React Testing Library](https://img.shields.io/badge/React%20Testing%20Library-E33332?style=for-the-badge&logo=testing-library&logoColor=white)](https://testing-library.com/docs/react-testing-library/intro)
[![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)](https://jestjs.io/)

### Utilities
[![React Hook Form](https://img.shields.io/badge/React_Hook_Form-FF6B6B?style=for-the-badge&logo=react&logoColor=white)](https://react-hook-form.com/)
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
