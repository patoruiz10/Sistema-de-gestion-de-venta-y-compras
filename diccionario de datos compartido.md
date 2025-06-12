# Diccionario de Datos

## Producto

```
Producto = CodBarra + CantStock + Desc + TipoProducto + Nombre + NomMarca
```

## TipoDeProducto

```
TipoDeProducto = [Bebidas | Mercadería | Cigarrillos | Limpieza | Comida | Golosinas | Medicamentos]
```

## MetodoPago

```
MetodoPago = [Efectivo | Transferencia | Débito | Crédito | QR]
```

---

## Proceso de Ventas

```
venta = MetodoPago + 1{ProdVen}n + PrecioTotal + 1{CantProd}n + FechaHora
PrecioTotal = PrecioUnit * CantProd
ProdVen = Nombre + Precio
```

---

## Tabla de Atributos

| Nombre        | Descripción                              | Longitud   | Tipo     | Dominio                                                                 |
|---------------|------------------------------------------|------------|----------|-------------------------------------------------------------------------|
| CodBarra      | Código identificatorio de producto        | 13 dígitos | Entero   | Continuo 0–99999999                                                     |
| Cant          | Cantidad de producto en stock             | 4 dígitos  | Entero   | Continuo                                                                |
| Desc          | Descripción del producto                  | 100        | String   | Continuo (texto libre)                                                  |
| TipoProducto  | Categoría de producto                     | 15         | String   | Discreto [Bebidas | Cigarrillos | Limpieza | Comidas | Golosinas | Medicamentos] |
| Nombre        | Nombre de producto                        | 50         | String   | Continuo (texto libre)                                                  |
| NomMarca      | Marca del producto                        | 50         | String   | Continuo (texto libre)                                                  |
| FechaHora     | Indicador del día y hora                  | datetime   | -        | Continuo                                                                |
| MetodoPago    | Forma de pago                             | 50         | String   | Discreto [Efectivo | Transferencia | Débito | Crédito | QR]           |
| Monto         | Precio del producto                       | 7 dígitos  | Double   | Continuo 0–9999999                                                      |

---

## Stock

```
Producto = CodBarra + TipoProducto + Nombre + NomMarca + Cant + Desc
```
