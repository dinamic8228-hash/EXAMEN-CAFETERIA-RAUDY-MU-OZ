# Cafetería El Buen Sabor — Pedidos

## 1. Datos del estudiante

- **Nombre:** Raudy Muñoz
- **Matrícula:** 2024-3943
- **Asignatura:** Programación Básica
- **Fecha:** 19/11/2026

## 2. Descripción del programa

Aplicación Windows Forms (C#) con un solo formulario (frmPedidos) que registra pedidos y calcula el total a pagar: adicional por tamaño grande y porción extra, descuento a clientes frecuentes, empaque para llevar e ITBIS del 18%.

## 3. Datos de entrada

- Cliente y si es frecuente. Fecha.
- Por producto: nombre y precio digitados, cantidad (1 a 20), tamaño y porción extra.
- Servicio: local o para llevar.

Precios de referencia (RD$): Café americano 75, Sándwich 180, Jugo 120, Pastelito 60, Batida 150.

## 4. Proceso

1. Precio unitario = precio + 25 si es grande + 30 si lleva porción extra.
2. Total de línea = precio unitario × cantidad. Subtotal = suma de líneas.
3. Descuento = 10% del subtotal si es frecuente.
4. Empaque = RD$20 una vez si es para llevar.
5. Base imponible = subtotal − descuento + empaque.
6. ITBIS = 18% de la base. Total = base + ITBIS.

## 5. Salida

- Lista del pedido en columnas (Cant, Producto, Precio, Total).
- Subtotal, descuento, empaque, ITBIS y total en formato RD$ 0.00.

Caso de prueba: María Pérez (frecuente); Sándwich 180 × 2 grande = 410.00; Jugo 120 × 1 con porción extra = 150.00; para llevar. Resultado: subtotal 560.00, descuento 56.00, empaque 20.00, base 524.00, ITBIS 94.32, **total RD$ 618.32**.

## 6. Capturas de pantalla

![Formulario con el caso de prueba](capturas/caso-prueba.png)

![Total calculado](capturas/total-calculado.png)
