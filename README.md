# Aplicaciones Web (next js, typescript, y docker)
Lenguaje de programacion: Typescript estricto.
Configuracion inicial para producir aplicaciones web *serverless* (sin servidor backend).

## Uso
```
  yarn 
  yarn dev
```

## Generar la imagen de docker
Primero ejecuta la aplicacion:
```
yarn
yarn build
yarn start
```

Cuando puedas correr exitosamente el servidor de nextjs, ahora si genera la imagen de docker:
```
  docker build -t next-prod-ts .
```

### Anexos: 
#### Arbol de archivos:
estructura de este proyecto
```
  |-- Dockerfile
  |-- README.md
  |-- next-env.d.ts
  |-- next.config.js
  |-- package.json
  |-- pages
  |   |-- _app.tsx
  |   |-- about.tsx
  |   |-- api
  |   |   `-- hello.ts
  |   |-- contact
  |   |   `-- index.tsx
  |   |-- index.tsx
  |   `-- pricing
  |       `-- index.tsx
  |-- postcss.config.json
  |-- public
  |   |-- favicon.ico
  |   `-- vercel.svg
  |-- src
  |   |-- components
  |   |   |-- ActiveLink.tsx
  |   |   |-- Navbar.module.css
  |   |   |-- Navbar.tsx
  |   |   |-- index.js
  |   |   `-- layouts
  |   |       |-- DarkLayout.tsx
  |   |       |-- MainLayout.module.css
  |   |       `-- MainLayout.tsx
  |   |-- containers
  |   |-- hooks
  |   |   |-- Counter.tsx
  |   |   `-- index.js
  |   `-- index.js
  |-- styles
  |   `-- globals.css
  -- tsconfig.json
```
