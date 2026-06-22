# 🧺 Sacos · Control de Deudas

App web privada para llevar el control de las ventas a crédito (venta de sacos):
quién me debe, cuánto, qué, desde cuándo y hasta cuándo debe pagar.

## Cómo se usa
- Abrir la página → ingresar usuario y contraseña.
- **+ Nueva deuda**: registrar cliente, monto, qué debe, fecha de ingreso y fecha de vencimiento.
- Cada deuda muestra su estado automático: **Al día**, **Por vencer** (≤7 días), **Vencida** o **Pagada**.
- **＋ Abono**: registrar pagos parciales; el saldo y la barra de progreso se actualizan solos.
- **💬 Cobrar**: abre WhatsApp con un mensaje de cobro listo (si guardaste el teléfono).
- KPIs arriba: total por cobrar, cuántos clientes deben, deudas por vencer y vencidas.
- **⤓ Respaldo**: descargar/restaurar todos los datos en un archivo `.json`.

## Notas técnicas
- 100% estático (HTML/CSS/JS en un solo archivo), sin servidor ni base de datos.
- Los datos se guardan en el **navegador** (localStorage) del dispositivo donde lo usas.
  Para no perderlos al cambiar de equipo o limpiar el navegador, usa **Respaldo** seguido.
- El login es del lado del cliente: protege de miradas casuales, no es seguridad de banco.
  No publiques datos sensibles aquí.
