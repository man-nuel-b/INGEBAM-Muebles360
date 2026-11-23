# Implementación y verificación · INGEBAM Muebles360

Aplicación autónoma de diseño paramétrico de mobiliario. Entrada: `index.html`, con módulos `furnitureCore.js`, `viewer.js`, `vision.js`, `photoStudio.js`, `renderer3d.js`, `quoteEngine.js`, `manufacturing.js` y `app.js`.

## Ejecución
Sirve el repositorio por HTTP, no con doble clic en `index.html`. Ejemplo local: `python -m http.server 8000` y abre `http://localhost:8000/`.

Publicación estática, si GitHub Pages está configurado: https://man-nuel-b.github.io/INGEBAM-Muebles360/

`server.js` es un componente independiente: GitHub Pages no ejecuta servidores Node. Cualquier función que dependa de ese backend requiere despliegue separado y configuración segura.

## Lista de pruebas antes de presentar a clientes
- Seleccionar dimensiones y verificar actualización consistente entre interfaz, despiece y cotización.
- Probar selector de acabados y rotación del visor.
- Cargar una imagen de referencia y comprobar validaciones y privacidad local.
- Exportar e importar un proyecto usando `ejemplo_proyecto.json` y revisar si se restauran todos los campos.
- Revisar tablas de corte y optimización, unidades y tolerancias.
- Ejecutar la batería de pruebas Node disponible (`tests.js`, `tests-v38.js`, `tests-manufacturing.js`), revisando sus requisitos de ejecución.
- Verificar consola, carga móvil y dependencias externas.

No se debe tratar un despiece o presupuesto demo como ingeniería de producción sin validación técnica. Los repositorios de ventanas e inmobiliaria permanecen independientes.