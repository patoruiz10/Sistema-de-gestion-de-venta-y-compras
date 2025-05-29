**DICCIONARIO DE DATOS:**

Producto = CodBarra+Cant+Desc+TipoProducto+Nombre+NomMarca  
TipoDeProducto = [Bebidas|Mercadería|Cigarrillos]

Mercadería = [Limpieza|Comida|Bebida|Golosinas|Medicamentos] 

Bebidas = NombreMarca+Producto  
Cigarrillos = Producto+NombreDeMarca+TipoDeCigarrillo

MetodoPago = [Efectivo|Transferencia| Débito| Crédito| QR ]
  
  
  *** PROCESO DE VENTAS***
  
venta = metodopago+producto+preciototal+cantProd+FechaHora
preciototal = preciounit*cant





| NOMBRE | DESCRIPCIÓN | LONGITUD | TIPO | DOMINIO |
| :---- | :---- | :---- | :---- | :---- |
| CodBarra | Código identificatorio de producto | 13 dígitos | entero | continuo 0-99999999 |
| Cant | Cantidad de producto en stock | 4 dígitos | entero | continuo |
| Desc | Descripción del producto | 100 | string | continuo (texto libre) |
| TipoDeProducto | Categoría de producto | 15 | string | discreto[Bebidas|Cigarrillos|Limpieza|Comidas|Golosinas|Medicamentos] |
| Nombre | Nombre de producto | 50 | string | continuo (texto libre) |
| NomMarca | Marca del producto | 50 | string | continuo (texto libre) |
| FechaHora | Indicador del dia y hora | datetime | \- | continuo |
| MetodoPago | Pago de productos | 50 | string | discreto [Efectivo|Transferencia| Débito| Crédito| QR] |
| Monto | Precio del producto | 7 dígitos | Double | Continuo 0-9999999 |


