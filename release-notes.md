# Release Notes — v1.0.0 (2025-10-03)

## Resumen
Lanzamiento inicial del **Gestor de Informes**, una herramienta web 100% offline creada para **organizar, filtrar y abrir enlaces de informes de bug bounty** sin depender de un backend. Ideal para paneles, PoCs, wikis, tickets y documentación interna. Todo queda guardado en `localStorage`, directamente en tu navegador.

## Problema que resuelve
En bug bounty y auditorías web, los informes suelen terminar repartidos entre wikis, tickets, pestañas del navegador y notas dispersas. Este gestor elimina ese caos con un entorno simple, visual y completamente local: clasificá, priorizá, anotá contexto y abrí informes individuales o en lote sin complicaciones.

## Qué aporta
- 🧠 **Orden quirúrgico**: categorías personalizadas (XSS, IDOR, RCE…) con títulos editables y URLs normalizadas.
- 🔍 **Búsqueda y filtro instantáneos**: buscador lateral por título, URL, nota o categoría.
- 📑 **Notas tácticas**: tooltip flotante con contexto, vista previa y última edición.
- ⚡ **Velocidad de ejecución**: abrir informes individuales o todos los filtrados (hasta 15 por clic).
- 🔁 **Exportación/Importación JSON**: copia o migra tu base con un clic.
- 🔒 **Privacidad y resiliencia**: sin backend ni conexión. Ideal para laboratorios y entornos sensibles.

## Características destacadas
- Crear, renombrar y eliminar categorías dinámicamente.
- Etiquetas de prioridad por informe: Leer inmediatamente, ahora, luego, buen informe, regular, montón.
- Modal de notas con vista previa segura (contenido escapado).
- Apertura masiva de informes filtrados con límite seguro.
- Carga masiva: pega múltiples URLs y crea renglones automáticamente.
- Búsqueda global con scroll suave al resultado.
- Persistencia automática en `localStorage`.

## Uso rápido
1. Abre el archivo `.html` en tu navegador.
2. Crea una categoría y empieza a agregar informes.
3. Asigna estados de prioridad y añade notas si lo necesitás.
4. Usá el filtro o el buscador global para encontrar rápidamente.
5. Abrí informes individuales o todos los filtrados con un clic.
6. Exportá/Importá tu base en JSON o reseteá todo si necesitás empezar de cero.

## Interfaz
- Tema oscuro con gradientes y glassmorfismo.
- Píldoras de estado con colores claros.
- Seguridad UI: notas escapadas (`<`, `>`, etc.) y apertura con `noopener,noreferrer`.

## Roadmap futuro
- 📁 Soporte para carpetas o colecciones dentro de categorías.
- 🔔 Sistema de recordatorios por fecha de informe.
- 🧪 Integración opcional con APIs externas (sin perder el modo offline).

## Licencia
- MIT — Uso responsable y legal únicamente.

---

*"Gestor de Informes — organiza, filtra y abre. Tu base de bug bounty, offline y al instante."*
