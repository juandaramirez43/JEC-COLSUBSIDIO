# JEC COLSUBSIDIO

Dashboard interno para consultar y consolidar información operativa del programa educativo JEC COLSUBSIDIO. La aplicación reúne datos almacenados en Google Sheets y Google Drive para facilitar el seguimiento de la operación por mes y colegio, y la generación de reportes.

## ¿Qué permite hacer?

- Consultar reportes del periodo seleccionado y filtrar la información por colegio.
- Revisar datos de seguimiento diario, novedades/listas, planeaciones, refrigerios y docentes.
- Consultar reportes de reemplazos y el historial de planeaciones.
- Identificar registros de niños con valores de asistencia en cero.
- Consultar respaldos de listas y descargar reportes para análisis o seguimiento.
- Explorar la interfaz con datos simulados o conectarla a un servicio de Google Apps Script.

Los reportes se presentan mediante indicadores y tablas. Su disponibilidad y contenido dependen de las hojas y carpetas configuradas en Google Drive y de las funciones implementadas en Apps Script.

## Componentes

- **Interfaz web:** React, TypeScript y Vite.
- **Servicio de datos:** Google Apps Script publicado como aplicación web.
- **Fuente de información:** Google Sheets y archivos de Google Drive.
- **Exportación de hojas de cálculo:** biblioteca `xlsx`.

La interfaz está en `src/` y el código del servicio de Apps Script en `google-apps-script/Code.gs`.

## Requisitos

- Node.js y npm.
- Una URL de aplicación web de Google Apps Script para consultar datos reales.
- Acceso a las hojas y carpetas de Google Drive que utiliza el servicio.

## Ejecución local

1. Clona este repositorio y entra en su carpeta.
2. Instala las dependencias:

   ```bash
   npm install
