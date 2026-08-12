# Chat bot cafetería La Finquita :sparkles: 

## Versión 2026 - Chat Bot :green_heart:




## 

*Bot conversacional que permite a los clientes de la cafetería La Finquita consultar el menú, armar un pedido y confirmarlo directamente desde Telegram, con seguimiento del estado de la orden hasta la cocina.*:sparkles:

 ¿Qué hace el sistema?

+ Da la bienvenida al cliente quien escribe al bot, distinguiendo si es un cliente nuevo o uno que ya había escrito antes.
+ Muestra el menú por categorías (Calientes, Panadería, Fríos) mediante botones interactivos.
+ Lista los productos de la categoría elegida, con nombre, precio y descripción.
+ Permite seleccionar productos por su número, agregándolos a un carrito de compra.
+ Suma automáticamente el total del pedido a medida que el cliente agrega productos.
+ Descuenta el stock disponible en el inventario cada vez que se agrega un producto.
+ Genera un número de pedido único cuando el cliente escribe "confirmar", cerrando la compra.
+ Guarda el pedido con su detalle, total, fecha y hora en la hoja de Pedidos.
+ (En construcción) Notifica a la cocina sobre el nuevo pedido y permite actualizar su estado ("En preparación", "En camino"), informando al cliente automáticamente.


## Citas

> Café con sabor dde campo y paz serena
> ~ La Finquita


## Tabla

| Herramienta| Version |
| ------------- |:-------------:|
| N8N   | Ultima versión  |
| Google Sheets | Ultima versión |
| Claude | Ultima versión |
| Git | Ultima versión |

## Blocks of code

```
Cliente escribe al bot
        │
        ├─ ¿Es la primera vez? → Registra usuario → Bienvenida
        │
        ├─ Elige categoría (botón) → Muestra productos numerados
        │
        ├─ Escribe el número del producto → Se agrega al carrito → Descuenta stock → Muestra total acumulado
        │
        └─ Escribe "confirmar" → Genera número de pedido → Guarda en hoja Pedidos → Avisa al cliente
```
