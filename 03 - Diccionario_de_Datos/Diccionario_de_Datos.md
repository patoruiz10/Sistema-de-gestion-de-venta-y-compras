**DICCIONARIO DE DATOS**

**PROCESO DE VENTAS:**
Venta \=  1{ProdVen}n \+ 1{CantProd}n \+ PrecioTotal \+ MetodoPago \+ FechaHora 
Preciototal \= PrecioUnit \* CantProd
ProdVen \= Descripcion \+ PrecioUnit
MetodoPago \= \[Efectivo| Transferencia| Débito| Crédito| QR \]

**STOCK:**
Producto = CodProducto + Categoria + Proveedor + Desc + PrecioUnitario + CantStock
Categoria \= \[Bebidas | Mercadería | Cigarrillos | Limpieza | Comida | Golosinas | Medicamentos]



| NOMBRE | DESCRIPCIÓN | LONGITUD | TIPO | DOMINIO |
| :---- | :---- | :---- | :---- | :---- |
| CodProducto | Identificador interno único del producto | 6 dígitos | entero | 1–999999 | 
| CantProd | Cantidad de producto en stock | 4 dígitos | entero | continuo |
| Desc | Descripción del producto | 100 | string | continuo (texto libre) |
| Categoría | Categoría de producto | 15 | string | discreto\[Bebidas\| Cigarrillos\| Limpieza\|Comidas\|Golosinas\|Medicamentos\] |
| FechaHora | Indicador del dia y hora | \- | datetime | continuo |
| MetodoPago | Pago de productos | 50 | string | discreto \[Efectivo\|Transferencia\|Débito\|Crédito\|QR\] |
| Proveedor | Nombre del proveedor asociado | 50 | string | continuo |
| PrecioUnit| Precio unitario del producto | 7 dígitos  | double   | continuo 0–9999999|
| CantStock | Cantidad de producto en stock | 4 dígitos  | entero   | continuo |


