---
title: React y MUI - Introducción
layout: home
nav_order: 2
---

# React y MUI - Introducción

React: Inicialización del proyecto
----------------------------------

{: .highlight }

>   React implementa la técnica web de desarrollo **Client Side Rendering (CSR)** donde el navegador carga archivos JavaScript, renderiza la página en el lado del cliente y envía un documento HTML completo al navegador para construir interfaces de usuario. 

1. Explore la documentación de [React](https://react.dev/) para comprender los conceptos básicos de esta biblioteca.
2. Cree un proyecto de React utilizando [Vite](https://vitejs.dev/guide/#scaffolding-your-first-vite-project).

   a) Dentro de la carpeta de su proyecto, abra la terminal y cree un nuevo proyecto de Vite con el siguiente comando:

    ```bash
      npm create vite@latest . 
    ```
   
   b) Seleccione el framework como :term:`React` y la variante como `TypeScript`.
   c) Instale las dependencias del proyecto e inicie el servidor de desarrollo con los siguientes comandos:

    ```bash
      npm install
      npm run dev
    ```

3. Compruebe la vista previa del resultado en el navegador.
4. Con un cliente de IAG, explique la estructura del proyecto en React, específicamente por el propósito de los archivos `index.html`, `src/main.tsx` y `src/App.tsx`.