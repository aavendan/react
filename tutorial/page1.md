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
    
    - Dentro de la carpeta de su proyecto, abra la terminal y cree un nuevo proyecto de Vite con el siguiente comando:

    ```bash
      npm create vite@latest . 
    ```
   
    - Seleccione el framework como :term:`React` y la variante como `TypeScript`.
    - Instale las dependencias del proyecto e inicie el servidor de desarrollo con los siguientes comandos:

    ```bash
      npm install
      npm run dev
    ```

3. Compruebe la vista previa del resultado en el navegador.
4. Con un cliente de IAG, explique la estructura del proyecto en React, específicamente por el propósito de los archivos `index.html`, `src/main.tsx` y `src/App.tsx`.

---

## React: App.tsx

1. Modifique el archivo `src/App.tsx` para mostrar un mensaje de bienvenida, por ejemplo:
    
    ```tsx
      
      ...

      function App() {
          return (
              <div>
                  <h1>Bienvenido al Dashboard</h1>
              </div>
          );
      }

      export default App;
      ```

2. Compruebe la vista previa del resultado en el navegador.
3. Utilice un cliente de IAG, para explicar cómo se renderiza el componente principal de la aplicación y `JSX`.

## MUI: Inicialización del proyecto y componente Grid

1. Explore la documentación de [MUI](https://mui.com/material-ui/getting-started/overview/) para comprender cómo integrar esta biblioteca en su proyecto de React.
2. Instale MUI y sus dependencias en su proyecto de React con el siguiente comando:

    ```bash
    npm install @mui/material @emotion/react @emotion/styled
    ```
3. Importe el componente `Grid` de MUI en su archivo `src/App.tsx` y utilícelo para crear una estructura básica de cuadrícula para su dashboard:

    ```tsx

      ...
      import { Grid } from '@mui/material';

      function App() {
         return (
            <Grid>

               {/* Encabezado */}
               <Grid>Elemento: Encabezado</Grid>

               {/* Alertas */}
               <Grid>Elemento: Alertas</Grid>

               {/* Selector */}
               <Grid>Elemento: Selector</Grid>

               {/* Indicadores */}
               <Grid>Elemento: Indicadores</Grid>

               {/* Gráfico */}
               <Grid>Elemento: Gráfico</Grid>

               {/* Tabla */}
               <Grid>Elemento: Tabla</Grid>

               {/* Información adicional */}
               <Grid>Elemento: Información adicional</Grid>

            </Grid>
         );
      }

      export default App;
      ```

4. Compruebe la vista previa del resultado en el navegador. 
5. Con un cliente de IAG, explique cómo se utiliza el componente `Grid` de MUI para crear una estructura de cuadrícula y cómo se pueden agregar elementos dentro de esta cuadrícula.
