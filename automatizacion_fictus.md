# Documentacion Tecnica: Cocina Fictus (Version Esencial)

Este documento detalla el funcionamiento del sistema digital desarrollado para Cocina Fictus, enfocado en la automatizacion de pedidos y el control de ventas para negocios locales.

## Arquitectura del Sistema

El sistema se divide en dos modulos principales:

1.  Módulo de Cliente (index.html): Catalogo digital optimizado para moviles con carrito de compras que genera pedidos estructurados para WhatsApp.
2.  Módulo Administrativo (admin.html): Panel en tiempo real para la gestion de ordenes, alertas sonoras y exportacion de datos para administracion externa.

---

## Plan Personalizado: Eficiencia y Control

| Debilidad Anterior | Solucion Fictus Esencial | Impacto en el Negocio |
| :--- | :--- | :--- |
| Falta de Control de Pedidos | Dashboard centralizado con estados (Recibido, Preparando, Listo). | Reduccion de errores en cocina y mejores tiempos. |
| Pedidos de WhatsApp Desordenados | Formato de mensaje estructurado con ID de Orden unico. | Facilita la identificacion de cada venta. |
| Dificultad para Auditar Ventas | Boton de exportacion a CSV (Excel) con un solo clic. | Reportes de ventas instantaneos para contabilidad. |
| Ventas Externas sin Registro | Modulo de Pedido Manual para ventas en local. | Centralizacion de todas las transacciones del dia. |

---

## Automatizaciones Implementadas

### 1. Sincronizacion de Pedidos
Cuando un cliente hace clic en "Enviar Pedido a WhatsApp":
- Se genera un ID unico (ej: ORD-A1B2C3).
- El pedido se registra en la base de datos local.
- La cocina recibe una alerta sonora instantanea.

### 2. Formato de WhatsApp
El mensaje que recibe el restaurante es limpio y profesional:
> Hola Cocina Fictus. Quisiera realizar el siguiente pedido (Cod: ORD-X1Y2Z3):
> - 2x Queso Relleno ($360.00)
> - 1x Orden de Panuchos ($120.00)
> Total: $480.00
> Direccion de entrega: [Escribe tu calle y colonia aqui]

### 3. Modulo de Exportacion (Excel/CSV)
Para mantener los costos bajos y la simplicidad, se ha integrado un boton de exportacion que genera un archivo compatible con Excel. Esto permite al dueño del negocio llevar sus ventas a su contador o software administrativo externo sin pagar por modulos complejos.

---

## Propuesta Comercial (Promocion 30% Off)

Al simplificar los modulos fiscales, podemos ofrecer este sistema como una "Herramienta de Operacion Vital" a un precio mas accesible:

- Inversion de Implementacion: $3,999 - $4,299 MXN.
- Incluye: Hosting en Cloudflare, Catalogo Digital, Panel de Cocina y Modulo de Exportacion.

---

## Guia de Uso

1.  Apertura: Iniciar el dia abriendo el /admin.html en una tablet con el volumen encendido.
2.  Preparacion: Al sonar la campana, cambiar el estado a "Cocinando".
3.  Cierre: Al final del dia, usar el boton "Exportar Ventas (CSV)" para guardar el registro del dia.

Propuesta de Valor: Este sistema transforma el desorden de WhatsApp en una linea de produccion eficiente y profesional.
