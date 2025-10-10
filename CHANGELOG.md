# Changelog

Todas las versiones siguen el formato [SemVer].

## [v1.0.0] - 2025-10-03
### Añadido
- Gestor de informes / URL — herramienta 100% offline para gestionar enlaces de bug bounty.
- Creación, renombrado y eliminación de **categorías personalizadas** (XSS, IDOR, RCE, etc.).
- **Gestión completa de renglones**: título editable, campo URL, apertura individual o en lote.
- Sistema de **etiquetas de prioridad** con colores claros:
  - 🔴 Leer inmediatamente  
  - 🟠 Leer ahora  
  - ⚪ Leer luego  
  - 🟢 Buen informe  
  - 🔵 Informe regular  
  - ⚪ Informe del montón
- **Notas con tooltip flotante**: contexto, fecha de última edición, vista previa segura.
- **Filtro instantáneo** por título, URL, nota o categoría.
- **Buscador global lateral** fijo con scroll suave al resultado.
- **Apertura masiva** (hasta 15 informes por clic) con aviso si quedan pendientes.
- **Carga masiva** desde texto plano (una URL por línea).
- **Exportación e importación JSON** para migrar tu base de datos de informes.
- **Reset total** (borrado nuclear) en un clic.
- Persistencia completa en `localStorage` sin backend ni instalación.
- Interfaz moderna con tema oscuro, gradientes y glassmorfismo.

### Cambiado
- N/A — primera versión estable.

### Corregido
- N/A — versión inicial.

### Notas
- Licencia: MIT.
- 100% offline, sin conexión ni dependencias externas.
- Los contenidos de notas y tooltips siempre se **escapan** (`<`, `>`, etc.) para prevenir XSS locales.
- El botón **Abrir** utiliza `noopener` y `noreferrer` para mayor seguridad.
