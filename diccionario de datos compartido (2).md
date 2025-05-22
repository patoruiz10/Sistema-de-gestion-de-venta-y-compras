

**DICCIONARIO DE DATOS:**

* Producto= CodBarra+Cant+Desc+TipoProducto+Nombre+NomMarca  
* Fecha=Dia+Mes+Año+Hora


| NOMBRE | DESCRIPCIÓN | LONGITUD | TIPO  | DOMINIO |
| ----- | ----- | ----- | ----- | ----- |
| CodBarra | Código identificatorio de producto | 13 dígitos  | entero | continuo 0-99999999 |
| Cant | Cantidad de producto en stock | 4 dígitos  | entero | continuo |
| Desc | Descripción del producto  | 100  | string | continuo (texto libre) |
| TipoDeProducto | Categoría de producto | 15 | string | \[Bebidas|Mercadería|Cigarrillos \] |
| Nombre | Nombre de producto  | 50 | string | continuo (texto libre) |
| NomMarca | Marca del producto | 50 | string | continuo (texto libre) |
| FechaHora  | Indicador del dia y hora  | datetime  | \- | continuo |
| Mercadería  | Sub categoría de producto  | 50 | string  | discreto\[Limpieza|Comida|Bebida|Golosinas|Medicamentos\]  |
| MetodoPago | Pago de productos | 50 | string | discreto \[Efectivo|Transferencia| Débito| Crédito| QR \] |
| Monto | Precio del producto | 7 dígitos | Double | Continuo  0-9999999 |
|  |  |  |  |  |





  ---


  **Ventas** 👍

  TipoDeProducto= \[Bebidas|Mercadería|Cigarrillos \]

  Mercadería= \[Limpieza|Comida|Bebida|Golosinas|Medicamentos\]

  MetodoPago= \[Efectivo|Transferencia| Débito| Crédito| QR \]

	venta=metodopago+producto+preciototal+cantProd  
	ticket= venta+preciototal  
	preciototal=preciounit\*cant

//Bebidas= Nombre de Marca+Producto  
//Cigarrillos \= Producto \+ NombreDeMarca \+ TipoDeCigarrillo

   
	STOCK

* Producto=CodBarra+TipoProducto+Nombre+NomMarca+Cant+Desc

