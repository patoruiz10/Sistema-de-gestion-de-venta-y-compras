# Caso de uso: Crear un nuevo usuario

* Actores primarios:  Encargado
* Actores secundario: No tiene
* Precondiciones: El usuario debe tener permisos para crear nuevo usuario
* Postcondiciones: El usuario se agrega a la lista de usuarios del sistema.

### Camino básico:

1. El encargado selecciona la opción “Crear nuevo usuario”.
2. El sistema muestra un formulario para ingresar los datos del nuevo usuario (nombre de usuario, contraseña, rol).
3. El encargado completa los datos solicitados y confirma la operación seleccionando la opción “Guardar”.
4. El sistema muestra un mensaje indicando que el usuario se creó correctamente, crea el nuevo usuario con los datos ingresados y lo agrega al listado de usuarios del sistema.



### Caminos alternativos:

4.a Existen campos obligatorios sin completar.  
4.a.1 El sistema muestra un mensaje indicando que faltan completar campos obligatorios.  
4.a.2 Vuelve al paso 3.

### Escenario de éxito:

* El encargado pudo crear un nuevo usuario en el sistema.

### Escenario de fracaso:

* El encargado no pudo crear el nuevo usuario porque dejó campos obligatorios sin completar.
