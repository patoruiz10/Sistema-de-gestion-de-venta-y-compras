**funcionales:**

- debe manejar el stock de la mercadería faltante   
- debe manejar stock de la mercadería disponible   
- la mercadería debe estar declarada por código de barra, cant existente, descripción, tipo de producto, nombre y nombre de marca  
- las ventas realizadas deben impactar en el stock  
- cuando se realiza reabastecimiento debe impactar en el stock


**no funcional:**

- debe tener dia, mes, año y hora, usuario del empleado, nombre del negocio: usabilidad  
- el reabastecimiento de los productos debe tener un tiempo de respuesta menor a 3 seg: eficiencia


**del dominio:**

- cada empleado debe contar con un usuario 

**DICCIONARIO DE DATOS:**

* Producto= CodBarra+Cant+Desc+TipoProducto+Nombre+NomMarca  
* Fecha=Dia+Mes+Año+Hora


| NOMBRE | DESCRIPCIÓN | LONGITUD | TIPO  | DOMINIO |
| ----- | ----- | ----- | ----- | ----- |
| CodBarra | código identificatorio de producto | 13 dígitos  | entero | continuo 0-99999999 |
| Cant | cantidad de producto en stock | 4 dígitos  | entero | continuo |
| Desc | descripción del producto  | 100  | string | continuo (texto libre) |
| TipoDeProducto | categoría de producto | 15 | string | \[Bebidas|Mercadería|Cigarrillos \] |
| Nombre | nombre de producto  | 50 | string | continuo (texto libre) |
| NomMarca | marca del producto | 50 | string | continuo (texto libre) |
| FechaHora  | indicador del dia y hora  | datetime  | \- | continuo |
| Mercaderia  | Sub categoría de producto  | 50 | string  | discreto\[Limpieza|Comida|Bebida|Golosinas|Medicamentos\]  |





  ---


  **Ventas** 👍

  TipoDeProducto= \[Bebidas|Mercadería|Cigarrillos \]

  Mercadería= \[Limpieza|Comida|Bebida|Golosinas|Medicamentos\]

  MetodoPago= \[Efectivo| MercadoPago| Transferencia| Débito| Crédito| QR \]


  


  

  //Bebidas= Nombre de Marca+Producto

  //Cigarrillos \= Producto \+ NombreDeMarca \+ TipoDeCigarrillo 