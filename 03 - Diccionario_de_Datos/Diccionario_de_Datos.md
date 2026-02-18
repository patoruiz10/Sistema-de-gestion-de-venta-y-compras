**DICCIONARIO DE DATOS**

**PROCESO DE VENTAS:**
Venta = 1{ProdVen}n + 1{CantProd}n + PrecioTotal + MetodoPago + FechaHora  
PrecioTotal = PrecioUnit \* CantProd  
ProdVen = CodProducto + Desc + PrecioUnit  
MetodoPago = \[Efectivo | Transferencia | Débito | Crédito | QR]

**STOCK:**
Producto = CodProducto + Categoria + Proveedor + Desc + PrecioUnitario + CantStock  
Categoria = \[Bebidas | Mercadería | Cigarrillos | Limpieza | Comida | Golosinas | Medicamentos]

|NOMBRE|DESCRIPCIÓN|LONGITUD|TIPO|DOMINIO|
|-|-|-|-|-|
|CodProducto|Identificador interno único del producto|6 dígitos|entero|1–999999|
|CantProd|Cantidad **vendida** del producto en la venta|4 dígitos|entero|discreto (>0)|
|Desc|Descripción del producto|100|string|continuo (texto libre)|
|Categoría|Categoría de producto|15|string|discreto \[Bebidas\|Cigarrillos\|Limpieza\|Comidas\|Golosinas\|Medicamentos]|
|FechaHora|Indicador del día y hora|-|datetime|continuo|
|MetodoPago|Pago de productos|50|string|discreto \[Efectivo\|Transferencia\|Débito\|Crédito\|QR]|
|Proveedor|**CUIT** del proveedor asociado|11 dígitos|entero|continuo|
|PrecioUnit|Precio unitario del producto|7 dígitos|double|continuo 0–9999999|
|CantStock|Cantidad de producto en stock|4 dígitos|entero|discreto (>=0)|



