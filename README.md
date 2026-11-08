# Agenda 90° Studio

## Uso rápido
1. Descomprime el ZIP.
2. Abre `index.html` en Chrome o Edge para usar la agenda.
3. Pulsa el botón ♬ o toca la pantalla una vez para habilitar el audio.
4. Crea sesiones desde **Nueva sesión**. Los datos se guardan en el almacenamiento local del navegador.
5. Usa **Exportar** para descargar un respaldo JSON e **Importar** para restaurarlo.

## Instalar como aplicación (PWA)
Para instalarla como aplicación en Windows, publica la carpeta en un hosting con HTTPS (por ejemplo, GitHub Pages o Hostinger) y abre la URL en Chrome/Edge. Usa el menú del navegador → Instalar página como aplicación. El service worker permite cargar los archivos básicos sin conexión después de la primera visita.

## Semáforo y alarma
- Verde: faltan 3 días o más.
- Amarillo: faltan 2 días.
- Rojo: falta 1 día o es hoy.
- Al abrir la agenda, se muestra alerta y se intenta reproducir un tono de emergencia de 10 segundos para sesiones de hoy o mañana. El navegador requiere interacción previa para habilitar audio.

## Importante
Esta es una primera versión local. Los datos permanecen en ese navegador y dispositivo; no hay sincronización entre equipos ni alarmas garantizadas con el navegador cerrado. Para notificaciones de fondo, sincronización y respaldo en la nube se necesita desplegar un backend y configurar notificaciones push.

## Pagos y facturas
- Cada sesión registra el valor total, el abono recibido y el saldo pendiente.
- El estado se calcula automáticamente: pendiente, abono recibido o pagado totalmente.
- En cada reserva usa **Factura PDF**. Se abre una factura imprimible con el nombre 90 Grados, consecutivo, datos del cliente, servicio, fecha, valor, abono y saldo.
- En el cuadro de impresión de Chrome/Edge elige **Guardar como PDF** y luego puedes compartir ese PDF por WhatsApp.
- Es un comprobante de servicio/pago de diseño tipo factura; no es una factura electrónica validada por la DIAN.


## Formato de factura actualizado
La factura se imprime en una sola página A4, sin páginas adicionales ni controles de pantalla. En el diálogo de impresión selecciona A4 y escala 100% o Ajustar al área imprimible si tu navegador lo requiere.

## Formato automático de valores
Los campos de precio y abono ahora agregan puntos de miles automáticamente según el formato colombiano (por ejemplo, 450.000). Los valores se guardan como números para cálculos y facturas.

## Módulo de finanzas
- Resumen de dinero recibido, valor total agendado y saldo pendiente por cobrar.
- Gráfico mensual de abonos/pagos recibidos, agrupado por año de la fecha de sesión.
- Detalle por cliente con valor, recibido y saldo pendiente.
- Búsqueda de clientes y exportación del detalle a CSV.
