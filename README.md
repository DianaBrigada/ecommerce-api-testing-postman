# Ecommerce API Testing – Postman Mock

Proyecto de **pruebas de API para un flujo de e-commerce** utilizando **Postman Mock Server**, enfocado en práctica QA.  
El proyecto no depende de un backend real.

---

## 🧰 Herramientas utilizadas
- Postman
- Postman Mock Server
- GitHub

---

## 🎯 Objetivo del proyecto
Validar el correcto funcionamiento de un flujo básico de e-commerce a nivel API, incluyendo:
- autenticación
- consulta de productos
- manejo de carrito
- creación y seguimiento de órdenes

---

## 📌 Alcance (Endpoints cubiertos)

1. **POST** `/auth/login`
2. **GET** `/products`
3. **POST** `/cart/items`
4. **GET** `/cart/{cartId}`
5. **POST** `/orders`
6. **POST** `/orders/{orderId}/pay`
7. **GET** `/orders/{orderId}`

---

## 📂 Estructura del repositorio
```
ecommerce-api-testing-postman/
├─ postman/
│ ├─ Ecommerce_API_Mock.postman_collection.json
│ └─ Ecommerce_Mock_ENV.postman_environment.json
├─ docs/
│ └─ TEST_PLAN.md
└─ README.md
```
---

- **postman/** → colección y environment exportados
- **docs/** → documentación del plan de pruebas

---

## ⚙️ Configuración

1. Importar en Postman:
   - `postman/Ecommerce_API_Mock.postman_collection.json`
   - `postman/Ecommerce_Mock_ENV.postman_environment.json`

2. Seleccionar el environment **Ecommerce Mock ENV**

3. Configurar la variable:
   - `baseUrl` = URL del Mock Server  

---

## ▶️ Ejecución de pruebas

- Ejecutar los requests manualmente en orden  
  **o**
- Usar **Collection Runner** para correr el flujo completo

---

## 🧪 Qué se valida

- Códigos de estado HTTP (200 / 201)
- Estructura de respuestas JSON
- Uso de variables entre requests:
  - `token`
  - `productId`
  - `cartId`
  - `orderId`
- Flujo end-to-end sin errores

---

## 📝 Notas
Este proyecto fue creado con fines de **práctica QA**, demostrando:
- uso de mocks
- pruebas funcionales de APIs
- documentación básica
- organización de repositorios en GitHub
