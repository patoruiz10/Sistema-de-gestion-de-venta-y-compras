**DICCIONARIO DE DATOS:**

| NOMBRE | DESCRIPCIÓN | LONGITUD | TIPO  | DOMINIO |
| ----- | ----- | ----- | ----- | ----- |
| CodBarra | código identificatorio de producto | 13 dígitos  | entero | continuo 0-99999999 |
| Cant | cantidad de producto en stock | 4 dígitos  | entero | continuo |
| Desc | descripción del producto  | 100  | string | continuo (texto libre) |
| TipoDeProducto | categoría de producto | 15 | string | \[Bebidas|Mercadería|Cigarrillos \] |
| Nombre | nombre de producto  | 50 | string | continuo (texto libre) |
| NomMarca | marca del producto | 50 | string | continuo (texto libre) |
| FechaHora  | indicador del dia y hora  | datetime  | \- | continuo |
| Mercadería  | Sub categoría de producto  | 50 | string  | discreto\[Limpieza|Comida|Bebida|Golosinas|Medicamentos\]  |
| MetodoPago | pago de productos | 50 | string | discreto \[Efectivo|Transferencia| Débito| Crédito| QR \] |


  ---


  **Ventas** 

  TipoDeProducto= \[Bebidas|Mercadería|Cigarrillos \]

  Mercadería= \[Limpieza|Comida|Bebida|Golosinas|Medicamentos\]

  MetodoPago= \[Efectivo|Transferencia| Débito| Crédito| QR \]

  //Bebidas= Nombre de Marca+Producto

  //Cigarrillos \= Producto \+ NombreDeMarca \+ TipoDeCigarrillo


   

 **STOCK**

* Producto=CodBarra+TipoProducto+Nombre+NomMarca+Cant+Desc  
* FechaHora=Dia+Mes+Año+Hora    
    
  