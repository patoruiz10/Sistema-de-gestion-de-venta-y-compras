# Caso de Uso del Proceso de Venta
### Actores
* Primarios: Propietarios del negocio, Empleados
### Precondiciones
El empleado debe estar logueado con su usuario.
### Postcondiciones
Se debe enviar a Arca un informe del comprobante con lo facturado en el día.

### Camino Básico
1. El empleado inicia el proceso de venta y carga el código de todos los productos a vender.
2. El sistema muestra por pantalla el monto total a pagar.
3. El empleado elige el método de pago que prefiera el cliente.
4. El sistema verifica el método de pago elegido y concreta la venta, guardando el comprobante emitido y registrando la venta.

### Caminos Alternativos
1.a El código de producto ingresado no está registrado en el sistema.  
1.a.1 El sistema muestra una alerta: "Código inexistente", vuelva al paso 1.  
3.a El método de pago no está disponible.  
3.a.1 El sistema muestra una alerta: "Método de pago no disponible", vuelva al paso 3.  
4.a El monto elegido no se puede concretar por fondos insuficientes.  
4.a.1 El sistema muestra un mensaje: "No es posible efectuar el pago", vuelva al paso 3.  
4.b El monto elegido no se puede concretar por tener que sustituir el método de pago elegido.  
4.b.1 El sistema muestra un mensaje: "Proceso de pago cancelado", vuelva al paso 3.

### Escenario de Éxito
El usuario realizó la venta y el registro de forma satisfactoria.

### Escenario de Fracaso
El usuario no pudo efectuar la venta.
