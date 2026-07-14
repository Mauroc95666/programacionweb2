# 🍞 gestion-panaderiakiataque-vue

Este repositorio contiene la plataforma web desarrollada con **Vue 3** y **Vite** diseñada para digitalizar y optimizar la gestión operativa de la **Panadería Kiataque**.

---

## 👥 Integrantes

| Integrante | Rol / Responsabilidad | GitHub |
| :--- | :--- | :--- |
| **Anderson Carvajal Romero** | Diseño de Interfaces & Frontend | [@anderson-carvajal](https://github.com) |
| **Marco Antonio Kiataque Uchiba** | Diseño de Interfaces & Frontend | [@antoniokiataque](https://github.com) |
| **Luis Portillo Gonzales** | Diseño de Interfaces & Frontend | [@luis-portillo](https://github.com) |

---

## 📑 Tabla de Contenidos

1. [Descripción del Proyecto](#-descripción-del-proyecto)
2. [Diseño de Interfaces](#-diseño-de-interfaces)
   - [Anderson Carvajal Romero (Pantallas 1 y 2)](#-anderson-carvajal-romero)
   - [Marco Antonio Kiataque Uchiba (Pantallas 3 y 4)](#-marco-antonio-kiataque-uchiba)
   - [Luis Portillo Gonzales (Pantallas 5 y 6)](#-luis-portillo-gonzales)
3. [Herramientas y Configuración Recomendada](#-herramientas-y-configuración-recomendada)
4. [Guía de Instalación y Configuración](#-guía-de-instalación-y-configuración)

---

## 📝 Descripción del Proyecto

La Panadería Kiataque gestiona actualmente sus operaciones de forma manual: los pedidos llegan por WhatsApp, las ventas se anotan en cuaderno y el control de insumos se lleva de memoria. Esto provoca quiebres de stock, pérdida de pedidos y dificultad para saber qué producto deja mayor ganancia.

**Nuestra solución:** El sistema propuesto centraliza productos, ventas, pedidos, inventario, clientes y reportes en una sola plataforma web, permitiendo que la panadería compita en condiciones equivalentes a las de empresas de mayor tamaño.

---

## 🎨 Diseño de Interfaces

A continuación se detallan los wireframes (esquemas de baja fidelidad) y mockups (diseños visuales finales) de las pantallas principales del sistema, organizados por el integrante responsable de su diseño:

### 👤 Anderson Carvajal Romero

#### 💻 Pantalla 1 — Inicio de Sesión
Autenticación de usuarios mediante correo electrónico y contraseña.

<table>
  <tr>
    <td align="center" width="50%"><b>Wireframe</b></td>
    <td align="center" width="50%"><b>Mockup</b></td>
  </tr>
  <tr>
    <td><img src="![](docs/mockups/01-login-wireframe.png)" alt="Wireframe — Inicio de Sesión" width="100%"/></td>
    <td><img src="docs/mockups/01-login-mockup.png" alt="Mockup — Inicio de Sesión" width="100%"/></td>
  </tr>
</table>

#### 📊 Pantalla 2 — Panel de Control
Visualización general del estado del negocio con indicadores de ventas, pedidos y stock.

<table>
  <tr>
    <td align="center" width="50%"><b>Wireframe</b></td>
    <td align="center" width="50%"><b>Mockup</b></td>
  </tr>
  <tr>
    <td><img src="docs/mockups/02-dashboard-wireframe.png" alt="Wireframe — Panel de Control" width="100%"/></td>
    <td><img src="docs/mockups/02-dashboard-mockup.png" alt="Mockup — Panel de Control" width="100%"/></td>
  </tr>
</table>

---

### 👤 Marco Antonio Kiataque Uchiba

#### 📦 Pantalla 3 — Catálogo de Productos
Gestión del catálogo de productos de la panadería.

<table>
  <tr>
    <td align="center" width="50%"><b>Wireframe</b></td>
    <td align="center" width="50%"><b>Mockup</b></td>
  </tr>
  <tr>
    <td><img src="docs/mockups/03-productos-wireframe.png" alt="Wireframe — Catálogo de Productos" width="100%"/></td>
    <td><img src="docs/mockups/03-productos-mockup.png" alt="Mockup — Catálogo de Productos" width="100%"/></td>
  </tr>
</table>

#### 🛒 Pantalla 4 — Punto de Venta
Registro rápido de ventas en mostrador.

<table>
  <tr>
    <td align="center" width="50%"><b>Wireframe</b></td>
    <td align="center" width="50%"><b>Mockup</b></td>
  </tr>
  <tr>
    <td><img src="docs/mockups/04-punto-venta-wireframe.png" alt="Wireframe — Punto de Venta" width="100%"/></td>
    <td><img src="docs/mockups/04-punto-venta-mockup.png" alt="Mockup — Punto de Venta" width="100%"/></td>
  </tr>
</table>

---

### 👤 Luis Portillo Gonzales

#### 🚚 Pantalla 5 — Pedidos y Delivery
Administración y seguimiento de pedidos realizados por los clientes.

<table>
  <tr>
    <td align="center" width="50%"><b>Wireframe</b></td>
    <td align="center" width="50%"><b>Mockup</b></td>
  </tr>
  <tr>
    <td><img src="docs/mockups/05-pedidos-wireframe.png" alt="Wireframe — Pedidos y Delivery" width="100%"/></td>
    <td><img src="docs/mockups/05-pedidos-mockup.png" alt="Mockup — Pedidos y Delivery" width="100%"/></td>
  </tr>
</table>

#### 📋 Pantalla 6 — Inventario
Control del stock de productos terminados e insumos.

<table>
  <tr>
    <td align="center" width="50%"><b>Wireframe</b></td>
    <td align="center" width="50%"><b>Mockup</b></td>
  </tr>
  <tr>
    <td><img src="docs/mockups/06-inventario-wireframe.png" alt="Wireframe — Inventario" width="100%"/></td>
    <td><img src="docs/mockups/06-inventario-mockup.png" alt="Mockup — Inventario" width="100%"/></td>
  </tr>
</table>

---

## 🛠️ Herramientas y Configuración Recomendada

Para un correcto desarrollo del proyecto, se sugiere configurar el entorno local con las siguientes herramientas:

### Configuración de IDE Recomendada
* **Editor de código:** [VS Code](https://code.visualstudio.com/)
* **Extensiones:** [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (se recomienda desactivar la extensión *Vetur* para evitar conflictos de sintaxis).

### Configuración Recomendada de Navegadores
* **Navegadores basados en Chromium (Chrome, Edge, Brave, etc.):**
  - Instalar [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd).
  - Activar [Custom Object Formatter en Chrome DevTools](http://bit.ly/object-formatters).
* **Firefox:**
  - Instalar [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/).
  - Activar [Custom Object Formatter en Firefox DevTools](https://fxdx.dev/firefox-devtools-custom-object-formatters/).

---

## 🚀 Guía de Instalación y Configuración

Sigue estos pasos para levantar el entorno de desarrollo localmente:

### 1. Clonar el repositorio
```sh
git clone [https://github.com/tu-usuario/gestion-panaderiakiataque-vue.git](https://github.com/tu-usuario/gestion-panaderiakiataque-vue.git)
cd gestion-panaderiakiataque-vue
```
### 2. Instalar dependencias del proyecto
```sh
npm install
```
### 3. Compilar y arrancar el servidor de desarrollo (Hot-Reload)
```sh
npm run dev
```
### 4. Compilar y minificar para producción
```sh
npm run build
```
### ⚙️ Configuración Adicional
Para más detalles sobre la configuración avanzada de compilación, consulta la Referencia de Configuración de Vite.
