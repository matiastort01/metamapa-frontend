# 🗺️ MetaMapa - Frontend (Cliente Liviano)

**Interfaz de usuario interactiva y Server-Side Rendering para la visualización de hechos geolocalizados.**

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Thymeleaf](https://img.shields.io/badge/Thymeleaf-%23005C0F.svg?style=for-the-badge&logo=Thymeleaf&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![Leaflet](https://img.shields.io/badge/Leaflet-199900?style=for-the-badge&logo=Leaflet&logoColor=white)

> 🔗 **Nota Arquitectura:** Este repositorio contiene exclusivamente el Cliente Liviano (Frontend). Para explorar la arquitectura de microservicios, la persistencia de datos y las APIs subyacentes, visitá el [Repositorio del Backend](https://github.com/matiastort01/metamapa-backend).

## 📌 Sobre el Proyecto

Este módulo representa la capa de presentación del ecosistema MetaMapa. Está diseñado como un cliente liviano estructurado bajo el patrón MVC, utilizando el motor de plantillas Thymeleaf y Spring Boot para el renderizado del lado del servidor (Server-Side Rendering).

Su objetivo principal es consumir las APIs unificadas del backend para brindar a los usuarios (visitantes, contribuyentes y administradores) una interfaz fluida, accesible y dinámica donde puedan visualizar, reportar y gestionar hechos en un mapa interactivo.

## 🖥️ Módulos y Funcionalidades Principales

* **Visualización Geoespacial:** Integración con la librería `Leaflet` mediante JavaScript para el renderizado interactivo de mapas, marcadores y pop-ups con información de los hechos.
* **Controladores de Presentación:** Lógica en Java (Spring MVC) encargada de interceptar las peticiones del usuario, comunicarse de forma segura con los microservicios del backend y orquestar las vistas correspondientes.
* **Gestión de Formularios:** Interfaces dinámicas para la ingesta de datos por parte de los contribuyentes, incluyendo soporte para contenido multimedia y validaciones de cliente/servidor.
* **Panel de Administración:** Vistas restringidas para perfiles autorizados que permiten visualizar estadísticas, revisar denuncias y moderar las colecciones de hechos.
* **Filtros Dinámicos:** Componentes de interfaz que permiten al usuario realizar búsquedas y cruces de datos por categorías, fechas y niveles de consenso directamente sobre el mapa.

## ⚙️ Características Técnicas Destacadas

* **Server-Side Rendering (SSR):** Generación de HTML dinámico en el servidor con Thymeleaf, mejorando la seguridad, el SEO y ocultando la lógica de consumo de APIs al cliente.
* **Desacoplamiento:** Total separación entre la capa visual y la lógica de negocio distribuida, favoreciendo la escalabilidad y el mantenimiento independiente.
* **Interactividad Asíncrona:** Uso estratégico de JavaScript vanilla para el manejo del DOM y las interacciones del mapa sin recargar la página completa.

## 🚀 Instalación Local

1. Clonar el repositorio:
   ```bash
   git clone [https://github.com/TU_USUARIO/metamapa-frontend.git](https://github.com/TU_USUARIO/metamapa-frontend.git)
   ```
   
2. Configurar las variables de entorno o el archivo application.properties para apuntar a la URL donde se esté ejecutando el Backend localmente.

3. Compilar el proyecto con Maven:
  ```bash
  mvn clean install
  ```

4. Iniciar el servidor embebido:
  ```bash
  mvn spring-boot:run
  ```
