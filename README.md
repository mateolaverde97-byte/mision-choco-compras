# Misión Chocó 2026 · Compras de materiales

Página de compras repartida por tienda: cada equipo compra en un tipo de tienda lo de todos los grupos (E1 mercería y papelería de oficina · E2 impresiones · E3 papelería escolar · E4 deportes y especializados · E5 variedades · Carlos y avanzada en Quibdó). Cada material indica el líder dueño. Registran comprado, cantidad, valor pagado, quién compró, notas y foto del recibo. Guarda en la hoja «Compras Chocó 2026» vía Apps Script.

Publicada en: `https://mateolaverde97-byte.github.io/mision-choco-compras/`

## Archivos
- `index.html`: la página completa (datos, diseño y lógica en un solo archivo).
- `apps-script/Compras.gs`: el backend para pegar en Apps Script.

## Conectar la hoja (una sola vez)
1. Abre la hoja **"Compras Chocó 2026"** → **Extensiones → Apps Script**. Borra lo que haya y pega todo `apps-script/Compras.gs`. Guarda.
2. Elige **setup** → **Ejecutar** → acepta los permisos (Hojas y Drive). Crea las pestañas `items` e `historial` y la carpeta de Drive «Recibos · Compras Chocó 2026».
3. **Implementar → Nueva implementación** → Aplicación web · Ejecutar como: **Yo** · Acceso: **Cualquier usuario** → Implementar.
4. Copia la URL que termina en `/exec` y pégala en `index.html` en `const API = '';`.

Mientras `API` esté vacío, la página funciona en modo prueba (guarda solo en el celular y no sube recibos).

## Si cambias el código de Apps Script
**Implementar → Gestionar implementaciones → editar (lápiz) → Versión: Nueva versión → Implementar.** La URL se mantiene.
