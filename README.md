# 🚀 QA Engineering: Pruebas de API - Urban Grocers (Sprint 4)

Este proyecto final completa mi **Employability Kit**, demostrando habilidades avanzadas en pruebas de servicios backend y validación de lógica de negocio a través de APIs.

## 🎯 Objetivo del Proyecto
Validar los endpoints de la API de Urban Grocers, centrándome en la gestión de kits de productos y la lógica de los servicios de entrega, asegurando que el servidor procese correctamente tanto las peticiones válidas como las erróneas.

## 🛠️ Tecnologías y Metodologías
* **Herramientas de Pruebas:** Postman para la ejecución de solicitudes HTTP.
* **Documentación Técnica:** Apidoc para la identificación de endpoints y estructuras JSON.
* **Gestión de Defectos:** Atlassian Jira para el reporte de fallos de API.
* **Tipos de Pruebas:** Pruebas positivas, negativas, Clases de Equivalencia y Valores Límite.

## 📁 Estructura del Repositorio
* **`/colecciones`**: Contiene el archivo JSON exportado de Postman.
* **`/documentacion`**: Incluye la hoja de cálculo con el diseño detallado de los casos de prueba.
* **`/evidencias`**: Capturas de pantalla de las respuestas del servidor y reportes de errores en Jira.

## 📊 Hallazgos Críticos (Jira)
Se documentaron errores de lógica importantes que afectan la integridad de los pedidos:
* **Falla de Validación (S4C5ES-9):** El sistema permite pedidos con cantidades de productos negativas, respondiendo que la entrega es posible.
* **Errores de Servidor (500 Internal Server Error):** Detectados al enviar datos inconsistentes en el ID del kit.

## 📝 Conclusión Técnica
Las pruebas revelaron que existen brechas de validación en el backend que permiten datos inconsistentes. Se recomienda implementar esquemas de validación de JSON más estrictos antes del despliegue final.
