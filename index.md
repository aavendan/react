---
title: React
layout: home
nav_order: 1
---

# Introducción a React

## ¿Qué es React?

React es una biblioteca de JavaScript desarrollada por Meta para construir interfaces de usuario interactivas y reutilizables.  
Se utiliza principalmente para crear aplicaciones web modernas basadas en componentes.

React permite desarrollar interfaces dinámicas de manera eficiente mediante la actualización selectiva del DOM utilizando un mecanismo conocido como **Virtual DOM**.

---

## Características principales de React

- Desarrollo basado en componentes reutilizables.
- Uso de JavaScript para construir interfaces.
- Actualización eficiente de la interfaz mediante Virtual DOM.
- Arquitectura declarativa.
- Amplio ecosistema y comunidad.
- Compatible con aplicaciones web y móviles.

---

## ¿Qué es un componente?

Un componente es una pieza reutilizable de la interfaz de usuario.  
Cada componente puede contener:

- Estructura HTML
- Estilos CSS
- Lógica JavaScript

Ejemplo conceptual:

```jsx
function Welcome() {
  return <h1>Hola React</h1>;
}
```

En este ejemplo:

- `function Welcome()` define un componente.
- `return` devuelve el contenido visual.
- `<h1>` representa el elemento que se mostrará en pantalla.

---

## JSX

React utiliza una sintaxis llamada **JSX** (*JavaScript XML*), que permite escribir estructuras similares a HTML dentro de JavaScript.

Ejemplo:

```jsx
const element = <h1>Bienvenido a React</h1>;
```

JSX facilita la lectura y organización de la interfaz de usuario.

---

## Virtual DOM

El **Virtual DOM** es una representación virtual del DOM real del navegador.

Proceso general:

1. React crea una copia virtual de la interfaz.
2. Detecta cambios en los componentes.
3. Calcula únicamente las diferencias necesarias.
4. Actualiza solo los elementos modificados en el navegador.

Esto mejora el rendimiento de la aplicación.

---

## Props

Las **props** (*properties*) permiten enviar información entre componentes.

Ejemplo:

```jsx
function Saludo(props) {
  return <h1>Hola {props.nombre}</h1>;
}

<Saludo nombre="Usuario" />
```

Resultado esperado:

```text
Hola Usuario
```

---

## Estado (State)

El **state** permite almacenar información que puede cambiar durante la ejecución de la aplicación.

Ejemplo:

```jsx
import { useState } from "react";

function Contador() {
  const [contador, setContador] = useState(0);

  return (
    <button onClick={() => setContador(contador + 1)}>
      {contador}
    </button>
  );
}
```

En este ejemplo:

- `useState(0)` crea una variable de estado.
- `contador` almacena el valor actual.
- `setContador()` actualiza el valor.

---

## Ventajas de React

| Ventaja | Descripción |
|---|---|
| Reutilización | Los componentes pueden reutilizarse en múltiples partes del proyecto |
| Escalabilidad | Facilita el desarrollo de aplicaciones grandes |
| Rendimiento | Optimiza actualizaciones mediante Virtual DOM |
| Comunidad | Posee gran cantidad de recursos y documentación |
| Ecosistema | Compatible con múltiples herramientas y librerías |

---

## Herramientas comunes en React

| Herramienta | Uso |
|---|---|
| Vite | Crear proyectos React rápidamente |
| React Router | Navegación entre páginas |
| Axios | Consumo de APIs |
| Tailwind CSS | Estilización rápida |
| Firebase | Backend y autenticación |

---

## Estructura básica de un proyecto React

```text
mi-app/
│
├── public/
├── src/
│   ├── components/
│   ├── App.jsx
│   ├── main.jsx
│   └── style.css
├── package.json
└── vite.config.js
```

---

## Flujo básico de trabajo en React

1. Crear el proyecto.
2. Diseñar componentes.
3. Construir la interfaz con JSX.
4. Manejar datos mediante props y state.
5. Consumir APIs.
6. Desplegar la aplicación.

---

## Ejemplo completo básico

```jsx
function App() {
  return (
    <div>
      <h1>Mi primera aplicación React</h1>
      <p>Bienvenido al desarrollo con React.</p>
    </div>
  );
}

export default App;
```

---

## Conclusión

React es una de las tecnologías más utilizadas para el desarrollo de interfaces modernas debido a su enfoque basado en componentes, su eficiencia y su facilidad para construir aplicaciones escalables e interactivas.