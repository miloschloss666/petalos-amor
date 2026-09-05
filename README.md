# 🌸 Pétalos y Amor – Sistema de Gestión Operativa

**Un software a medida para transformar la gestión de una floristería tradicional en un negocio digital, eficiente y conectado.**

---

## 📖 Introducción

**Pétalos y Amor** es una floristería ubicada en Maicao, La Guajira, que ha crecido en popularidad gracias a la calidad de sus arreglos florales y la cercanía con sus clientes. Sin embargo, este crecimiento también trajo consigo problemas operativos que afectan la experiencia del cliente y la eficiencia interna:

- Errores frecuentes en las entregas por direcciones incompletas o incorrectas.
- Falta de comunicación entre el equipo de ventas, los floristas y los mensajeros.
- Descontrol en el inventario, provocando roturas de stock o excesos de producto.
- Notificaciones inexistentes para los clientes, que desconocen el estado de sus pedidos.
- Rutas improvisadas por parte de los mensajeros, generando demoras y quejas.

Frente a este escenario, **nace el Sistema de Gestión Operativa para Pétalos y Amor**, una solución tecnológica integral que automatiza y organiza cada paso del proceso: desde que el cliente hace un pedido hasta que recibe sus flores en la puerta de su casa.

---

## 🎯 Objetivos del Proyecto

### Objetivo General

Diseñar, desarrollar e implementar un sistema de gestión operativa que permita a la floristería **Pétalos y Amor** optimizar sus procesos de ventas, inventario, logística y comunicación, reduciendo errores, mejorando la experiencia del cliente y aumentando la eficiencia del equipo.

### Objetivos Específicos

- **Digitalizar el registro de pedidos** con validación de stock en tiempo real.
- **Controlar el inventario** de productos e insumos mediante alertas automáticas de reabastecimiento.
- **Notificar al cliente** por SMS o WhatsApp en cada cambio de estado del pedido.
- **Proveer una app móvil** para que los mensajeros reciban rutas óptimas y confirmen entregas con un solo clic.
- **Generar reportes** de ventas, productos más vendidos, eficiencia de mensajeros y quejas.
- **Asegurar la información** mediante roles de acceso (Administrador, Vendedor, Mensajero).

---

## 🔍 Problemas Identificados (Diagnóstico)

| Área | Problema | Consecuencia |
| :--- | :--- | :--- |
| **Pedidos y entregas** | Direcciones incorrectas o incompletas. | Devoluciones, retrasos y clientes insatisfechos. |
| **Inventario** | Control manual y desactualizado. | Pérdida de ventas por falta de stock o desperdicio. |
| **Logística** | Mensajeros improvisan rutas. | Entregas tardías y mayor consumo de combustible. |
| **Comunicación** | Falta de notificaciones al cliente. | Incertidumbre y quejas recurrentes. |
| **Seguridad** | Acceso sin restricciones a datos sensibles. | Riesgo de filtración de precios y ganancias. |

---

## ✅ Alcance del Proyecto

### El Sistema Incluye

- **Módulo de Pedidos**: Registro, seguimiento y anulación (con justificación) de pedidos.
- **Módulo de Inventario**: Control de stock de productos (arreglos) e insumos (flores sueltas, cintas, etc.).
- **Módulo de Notificaciones**: Envío automático de SMS/WhatsApp al cliente (preparación, envío, entregado).
- **App Móvil para Mensajeros**: Visualización de rutas óptimas y confirmación de entregas (integrado con Mapbox).
- **Módulo de Reportes**: Generación de informes de ventas, productos, eficiencia y quejas.
- **Módulo de Usuarios y Roles**: Gestión de empleados con permisos diferenciados.

### El Sistema NO Incluye

- Procesamiento directo de pagos electrónicos (solo registro del método de pago).
- Gestión de nómina o contabilidad.
- Control automatizado de compras a proveedores.
- Marketing masivo o envío de correos electrónicos.

---

## 🏗️ Arquitectura y Tecnologías

### Arquitectura General

- **Cliente-Servidor de 3 capas** (Presentación, Lógica de Negocio, Datos).
- **Web + App Móvil** con comunicación mediante API REST.

### Tecnologías Seleccionadas

| Capa | Tecnología | Justificación |
| :--- | :--- | :--- |
| **Backend** | Node.js con Express / Django (Python) | Alto rendimiento, gran ecosistema y fácil integración con servicios externos. |
| **Base de Datos** | PostgreSQL 15 / MySQL 8.0 | Gratuitas, robustas y con soporte para transacciones ACID. |
| **Frontend Web** | React.js / Vue.js | Interfaces rápidas y responsivas, con alta reutilización de componentes. |
| **App Móvil** | Kotlin (Android nativo) | Mejor rendimiento y acceso directo a hardware (GPS, cámara). |
| **Mapas** | Mapbox SDK (Plan gratuito) | 50,000 map loads/mes sin costo, más económico que Google Maps. |
| **Servidor** | Ubuntu 22.04 LTS + Nginx | Estable, gratuito y con amplia documentación. |
| **Versionamiento** | Git + GitHub | Control de cambios colaborativo y trazabilidad. |

---

## 📦 Módulos Funcionales del Sistema

| Módulo | Descripción | Usuarios Involucrados |
| :--- | :--- | :--- |
| **Autenticación** | Inicio de sesión, recuperación de contraseña y gestión de sesiones. | Todos los usuarios. |
| **Pedidos** | Registro, consulta, anulación (con justificación) y cambio de estado. | Vendedores, Administradores. |
| **Inventario** | Visualización, actualización de stock y alertas de productos críticos. | Vendedores, Administradores. |
| **Logística (App Móvil)** | Visualización de rutas, mapas y confirmación de entregas. | Mensajeros. |
| **Notificaciones** | Envío automático de estados del pedido al cliente (vía SMS/WhatsApp). | Sistema (automático). |
| **Reportes** | Generación de informes en PDF/CSV con métricas clave. | Administradores. |
| **Usuarios y Roles** | Creación, edición y asignación de permisos a empleados. | Administradores. |

---

## 👥 Equipo de Trabajo y Metodología

- **Metodología:** Scrum (entregas cada 2 semanas, revisión con el cliente).
- **Duración estimada:** 3 meses (12 semanas – 4 sprints).
- **Equipo:**
  - **Andrés Camilo Villa Ruiz** – Desarrollo Backend / Base de Datos.
  - **Sharíth Milena Illidge Macea** – Desarrollo Frontend / App Móvil.
  - **Pedro Pimienta** – Instructor y asesor técnico.
  - **Sra. María López** – Cliente / Dueña de la floristería (validación y retroalimentación).

---

## 📈 Impacto Esperado

Con la implementación de este sistema, se espera:

- **Reducción del 80% de errores en entregas** gracias a la validación de direcciones.
- **Aumento del 40% en la satisfacción del cliente** por las notificaciones en tiempo real.
- **Mejora del 60% en la eficiencia logística** al eliminar rutas improvisadas.
- **Control total del inventario**, reduciendo pérdidas por productos vencidos o faltantes.
- **Toma de decisiones basada en datos** mediante reportes automáticos y precisos.

---

## 📌 Estado del Proyecto

- ✅ **Fase de Análisis** (RA1, RA2, RA3 de 1093 y 1094) – Completada.
- ✅ **Fase de Diseño** (RA1, RA2, RA3 de 1095) – En proceso de validación.
- ⏳ **Fase de Construcción** (RA1, RA2, RA3 de 1096) – Planificación y codificación.
- ⬜ **Fase de Pruebas y Despliegue** – Pendiente.

---

## 📄 Licencia

Este proyecto es desarrollado con fines académicos y educativos bajo la supervisión del **SENA – Centro Industrial y de Energías Alternativas**. Todo el código y la documentación son propiedad de los autores, con licencia de uso para la floristería **Pétalos y Amor**.

---

**¿Quieres saber más?**  
Contáctanos:  
- Andrés Camilo Villa Ruiz – `acvillar@soy.sena.edu.co`  
- Sharíth Milena Illidge Macea – `smillidge@soy.sena.edu.co`

---

*🌷 "Porque cada flor merece un camino seguro hasta quien la espera."*