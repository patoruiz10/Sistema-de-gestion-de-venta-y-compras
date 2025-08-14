# Caso de uso: Apertura de Caja
* Actores primarios: Empleado, Encargado
* Actores secundarios: No tiene
* Precondición: El usuario debe tener permisos
* Postcondición: No tiene

### Camion Básico
* El usuario selecciona la opción de “Apertura Caja”.
* El sistema muestra un mensaje para ingresar las credenciales.
* El usuario se loguea con sus credenciales.
* El sistema verifica las credenciales del usuario, abre la caja y muestra una alerta con un mensaje “Se abrió la caja correctamente (fecha del día y hora)”

### Caminos alternativos:
4.a Las credenciales ingresadas son incorrectas o no tiene permisos para ingresar al sistema.  
4.a.1 El sistema no pudo corroborar correctamente las credenciales ingresadas entonces se muestra una alerta: “Las credenciales ingresadas son incorrectas o no tiene permisos.” en la que solicita las credenciales nuevamente.  
4.a.2  Vuelve al paso “3”.

### Escenario de éxito: 
* El usuario pudo realizar la apertura de caja efectivamente.

### Escenario de fracaso: 
* El usuario no pudo realizar la apertura de caja.