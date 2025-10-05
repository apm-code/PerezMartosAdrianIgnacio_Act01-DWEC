# Actividad 1. Carrito de la compra aGoodShop

**Desarrollo Web en Entorno Cliente (DWEC)**   
**Adrián Ignacio Pérez Martos** 
**2º DAW** 

---

## Descripción

Este proyecto corresponde a la actividad 1 del módulo DWEC.  
El objetivo era implementar la funcionalidad de un carrito de compra a partir de una API externa, aplicando **Programación Orientada a Objetos (POO)** y **manipulación del DOM** en JavaScript.

La aplicación permite visualizar productos obtenidos desde una API, modificar las cantidades y ver el **total del carrito** actualizado dinámicamente.

---

## Estructura del proyecto

- `index.html` → Maquetación principal del proyecto, estructurada con **Bootstrap** para lograr un diseño adaptable y limpio.  
- `style.css` → Hoja de estilos personalizada para mejorar la presentación general.  
- `scripts.js` → Contiene toda la lógica del carrito.  
  > Ha sido necesario el cambio de la API a mocki.io.

---

## API utilizada

Originalmente, la práctica proponía usar [jsonblob.com](https://jsonblob.com), pero al no funcionar, se sustituyó por **[Mocki.io](https://mocki.io/)**:

```js
fetch("https://mocki.io/v1/9a926951-f996-4b80-aa33-26cd10b2312a")
```

El JSON contiene la divisa y los productos simulados de la tienda:

```json
{
  "currency": "€",
  "products": [
    {
      "SKU": "CAT1PLUSH01",
      "title": "Peluche de gato sonriente",
      "price": "19.95"
    },
    {
      "SKU": "CAT2MUG02",
      "title": "Taza con orejas de gato",
      "price": "14.50"
    },
    {
      "SKU": "CAT3MAT03",
      "title": "Alfombrilla de ratón con forma de patita",
      "price": "9.95"
    },
    {
      "SKU": "CAT4LAMP04",
      "title": "Lámpara de gato dormilón",
      "price": "29.95"
    },
    {
      "SKU": "CAT5NOTE05",
      "title": "Bloc de notas con diseño de gatos",
      "price": "6.95"
    }
  ]
}
```

---

## Aspectos trabajados

- Uso de una **clase Carrito** para gestionar los productos y el total.
- Uso de **métodos encapsulados** y manipulación de colecciones (`Map`).
- **Eventos DOM** para actualizar cantidades y precios dinámicamente.
- Rediseño del **HTML**.
- Integración de **Bootstrap** y **CSS** para mejorar la legibilidad y aspecto.
- Incorporación de un **footer** con estilo coherente al conjunto.
- Maquetación **responsive**.

---
