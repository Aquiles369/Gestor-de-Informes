# Política de seguridad

## 🧠 Resumen

Este proyecto — **Gestor de Informes** — es una herramienta **100% offline** diseñada para organizar y gestionar enlaces e informes de bug bounty directamente desde el navegador, **sin conexión a Internet ni backend**.  
Todo se almacena localmente mediante `localStorage`, lo que reduce la superficie de ataque y la exposición de datos sensibles.

---

## 🔒 Principios de seguridad

- **Sin backend ni red:** todos los datos permanecen en tu navegador y nunca se envían a servidores externos.
- **Persistencia local:** la información (categorías, informes, notas, estados) se guarda solo en `localStorage`.
- **Contenido escapado:** todos los textos mostrados (notas, tooltips, títulos) se escapan (`<`, `>`, `&`, etc.) para prevenir ejecución accidental de código (p. ej., XSS local).
- **Apertura segura de URLs:** el botón “Abrir” utiliza `noopener` y `noreferrer` para evitar ataques de `window.opener` y fugas de referencia.
- **Cero dependencias externas:** no se cargan librerías de terceros desde CDNs. Todo el código se ejecuta localmente.
- **Modo laboratorio:** pensado para entornos aislados, análisis en red local y uso en laboratorios de seguridad.

---

## ⚠️ Buenas prácticas recomendadas

- Usar siempre la herramienta en **entornos controlados** o en tu máquina local.
- **No almacenar** información extremadamente sensible (credenciales, tokens, datos personales) en notas, ya que se guardan en `localStorage`.
- Exportar el archivo JSON de forma segura si vas a compartirlo. No publiques contenido sensible en repositorios públicos.
- Borrar o restablecer (`reset total`) la base de datos antes de compartir la herramienta con otros usuarios o cambiar de entorno.
- Mantener actualizado el navegador para beneficiarte de parches de seguridad recientes.

---

## 🐛 Reporte de vulnerabilidades

Si encontrás un problema de seguridad en el proyecto (por ejemplo, bypass de escapado, comportamiento inesperado o riesgo potencial), por favor informalo siguiendo estos pasos:

1. No abras un *issue* público.
2. Enviá un mensaje privado al autor del repositorio a través de GitHub o Discord.
3. Incluí una descripción detallada del problema, pasos para reproducirlo y contexto del entorno donde fue detectado.

Intentaremos evaluar y solucionar cualquier problema reportado **lo antes posible**.

---

## 🛠️ Alcance del modelo de seguridad

| Área                              | Estado                         |
|----------------------------------|-------------------------------|
| Backend / API                    | ❌ No aplica (no existe)      |
| Base de datos remota            | ❌ No aplica                  |
| Persistencia local (`localStorage`) | ✅ Soportada y protegida      |
| Sanitización de contenido       | ✅ Escapado automático        |
| Dependencias externas           | ✅ Sin dependencias externas  |
| Navegación / apertura de URLs   | ✅ `noopener`, `noreferrer`   |

---

## 🧪 Nota importante

Esta herramienta está pensada **para uso ético y educativo** en contextos de bug bounty, pentesting y auditorías controladas. No debe utilizarse para actividades ilegales o sin autorización.

---

**“La mejor herramienta es la que no deja fugas. El Gestor de Informes vive en tu navegador, y no sale de ahí.”**
