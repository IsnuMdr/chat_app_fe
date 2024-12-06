# Simple Chatting App with GraphQL

## Preview

![Screenshot 2024-12-06 101406](https://github.com/user-attachments/assets/cdf3004d-8fa8-4de6-a183-785dce78e9a8)
![Screenshot 2024-12-06 101458](https://github.com/user-attachments/assets/e0bdcf31-b679-4375-b132-f40df954b18a)
![Screenshot 2024-12-06 101512](https://github.com/user-attachments/assets/c639f5eb-aad9-44fd-a8c2-7d7e1c2cc4ba)
![Screenshot 2024-12-06 101522](https://github.com/user-attachments/assets/e3aeeb74-6cf2-4a1a-b766-e9452892b6fa)

## Instalation
### Clone and Install This Repo for API
- [API for Chat APP With Nest Js](https://github.com/IsnuMdr/chat_app_api)

### Install
` npm install `

### Configure URI WebSocket
Configure URI WebSocket in `.src/apolloClient.ts` to URI your backend. 

### Run App
` npm run dev `

# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

- Replace `tseslint.configs.recommended` to `tseslint.configs.recommendedTypeChecked` or `tseslint.configs.strictTypeChecked`
- Optionally add `...tseslint.configs.stylisticTypeChecked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and update the config:

```js
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  // Set the react version
  settings: { react: { version: '18.3' } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs['jsx-runtime'].rules,
  },
})
```
