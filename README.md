# 🍃 Fruta de Calidad — PWA MVP

PWA estática y responsive para validar compras agrupadas de fruta en condominios de Lima.

## Funciones implementadas
- Catálogo de 8 frutas con precios ilustrativos y carrito de compra.
- Selección de condominio piloto, torre/departamento y datos de recepción.
- Registro local de pedidos de prueba, guardados en `localStorage` del **mismo navegador**.
- Vista de shopper: consolidación de cantidades y marcado de pedidos preparados.
- Vista de taxista: agrupación por condominio, enlace a Google Maps para cada destino y cambios de estado.
- Vista administrativa: indicadores básicos y pedidos.
- Manifest y service worker para instalación y consulta offline de la interfaz.
- Diseño adaptable a celulares.

## IMPORTANTE: no es un sistema de ventas en producción
**Es un prototipo sin backend.** Los roles son un selector de demostración, no hay autenticación ni controles de acceso. Los pedidos no se sincronizan entre equipos; se quedan en el navegador donde se registran. No existe integración real de Yape/Plin, pasarela de pagos, mensajes ni asignación automática de rutas. Google Maps solo abre un destino; no optimiza paradas. **No se deben usar datos personales reales** hasta implementar backend seguro, consentimiento, controles de privacidad y retención.

## Publicación con GitHub Pages
En el repositorio, abrir **Settings → Pages → Build and deployment**, seleccionar **Deploy from a branch**, rama `main`, carpeta `/(root)` y guardar.
La URL esperada, una vez GitHub Pages termine de publicar, es `https://gianpierrecalderon123.github.io/frutadecalidad/`.

## Siguiente fase antes del piloto
1. Autenticación y roles reales (residente, shopper, conductor, administrador).
2. Backend, base de datos, catálogo y precios administrables.
3. Alta de condominios con verificación y aceptación de recepción.
4. Reglas de cierre de pedidos por fecha/ruta, disponibilidad y sustituciones de fruta.
5. Optimización con Google Maps Route Optimization API desde servidor, con cuota y credenciales protegidas.
6. Pagos, conciliación, devoluciones y facturación según régimen tributario.
7. Privacidad, eliminación de datos, comprobante de entrega, auditoría y reportes de merma.
