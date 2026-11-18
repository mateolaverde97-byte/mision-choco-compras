# Misión Chocó 2026 · Compras de materiales

Página para que cada equipo registre sus compras: check de comprado, cantidad, valor pagado, quién lo compró, notas y foto del recibo. Los materiales de Quibdó y la partida de dulces quedan en el grupo «Carlos · avanzada». Se publica en GitHub Pages y guarda en la hoja «Compras Chocó 2026» a través de Apps Script.

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
