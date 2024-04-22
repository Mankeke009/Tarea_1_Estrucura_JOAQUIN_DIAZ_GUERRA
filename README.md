# Codigo para gestion hospitalaria 
Este es un sistema de gestión hospitalaria desarrollado en lengguaje de programacion C, en este se permite hacer diversas operaciones que ayudan a la administracion en una lista de espera de pacientes. 
## Funciones usadas:
1. **largo_lista**: Esta funcion se encarga de retornar el valor del largo de la lista (dar cuanto mide la lista). 

2. **mayus**: Esta funcion se encarga de convertir todas las letras de la cadena en mayusculas.

3. **cmp**: Esta funcion se encarga de ordenar la lista en base  a alta, media, baja y si es que alguna de estas se repite ordenarla por la hora.
4. **mostrar_paciente**: Esta funcion se encarga de mostrar el paciente solicitado.
5. **registrar_paciente**: Esta funcion permite registrar un nuevo paciente y colocarlo a la lista de espera.
6. **asignar_prioridad**: Esta funcion se encarga de asignar la prioridad del paciente que quieras y si este no existe se muestra un aviso.
7. **mostrarMenuPrincipal**: Esta funcion se encarga de mostrar el menu princiopal para que elijas una opcion.
8. **mostrar_lista**: Esta funcion se encarga de mostrar la lista de espera con los datos de cada paciente.
9. **atender_paciente**: Esta funcion selecciona al siguiente paciente a ser atendido según el orden de prioridad y lo elimina de la lista de espera y ademas muestra los datos del paciente. Si no quedan pacientes se muestra un aviso.
10. **mostrar_por_prioridad**: Esta funcion se encarga de mmostrar los pacientes de la prioridad que deseas ver.

## Funcionalidades : 
### Funcionando correctamente:

- Registrar pacientes con sus datos básicos y una prioridad inicial.
- Asignar o modificar la prioridad de los pacientes.
- Ver la lista de espera de pacientes, ordenada por prioridad y hora de registro.
- Atender al siguiente paciente, respetando el orden de prioridad.
- Mostrar la lista de pacientes por prioridad.
### A mejorar:
- Al escrbir un dato no relacionado del que te piden volver a pedirlo
- Implementar una interfaz de usuario más amigable.
- Permitir la edición de los datos de los pacientes.
  
## Ejemplo/Instrucciones de uso:
mientras el usuario ingrese los datos como se le solicitan todo funcionara bien.  
1. Ingresa la opcion que quieras usar si usas una no valida se te avisara
````
******************************************
     Sistema de Gestión Hospitalaria
******************************************

1. Registrar paciente
2. Asignar prioridad a paciente
3. Mostrar lista de espera
4. Atender al siguiente paciente
5. Mostrar pacientes por prioridad
6. Salir

------------------------------------------
Ingrese su opción:
````
2. Si elijes la opcion 1 debes darle los datos del paciente (nombre,edad,sintoma) en el orden que te acabo de decir.
````
Ingrese su opción: 1
Ingrese el nombre del paciente: joaquin
Ingrese la edad del paciente: 20
Ingrese sintoma del paciente: tos

--------------------------
Nombre: joaquin
Edad: 20
Sintoma: tos
Hora de llegada: 20:39:30
Prioridad: BAJA
--------------------------
````
3. Si elijes la opcion 2 debes ingresar el nombre del paciente que deseas buscar y luego asignar su nueva prioridad (alta,media,baja) en mayusuclas o minusculas pero solo esas palabras,ademas de asignarle su nuevo lugar en la fila ,si no se encuentra el paciente o no existen pacientes se te avisara.
````
Ingrese su opción: 2
Nombre del paciente a buscar:cynthia
Paciente encontrado
Prioridad a asignar:alta

PRIORIDAD ASIGNADA:
--------------------------
Nombre: cynthia
Edad: 50
Sintoma: tos
Hora de llegada: 20:50:29
Prioridad: ALTA
--------------------------
````
4. Si elijes la opcion 3 te mostrar la lista de espera.
````
Ingrese su opción: 3

LISTA DE PACIENTES:

--------------------------
Nombre: cynthia
Edad: 50
Sintoma: tos
Hora de llegada: 20:50:29
Prioridad: ALTA
--------------------------
--------------------------
Nombre: joaquin
Edad: 20
Sintoma: tos
Hora de llegada: 20:49:25
Prioridad: BAJA
--------------------------
--------------------------
Nombre: samuel
Edad: 20
Sintoma: fiebre
Hora de llegada: 20:49:42
Prioridad: BAJA
--------------------------
````
5. Si elijes la opcion 4 mostrara al paciente en la primera posicion de la fila, ademas de sacarlo de la lista, en caso de no quedar pacientes se dara aviso, y si es que quedan pacientes se dira cuantos quedan.
````
Ingrese su opción: 4
PACIENTE A ATENDER:
--------------------------
Nombre: joaquin
Edad: 20
Sintoma: tos
Hora de llegada: 20:49:25
Prioridad: BAJA
--------------------------
No quedan pacientes en espera
````
6. Si elijes la opcion 5 debes ingresar la prioridad que deseas ver (alta,media,baja) en mayusuclas o minusculas pero solo esas palabras,luego se te mostrara una lista de los pacientes de la prioridad elejida.
````
Ingrese su opción: 5
Que prioridad desea ver:baja

--------------------------
Nombre: joaquin
Edad: 20
Sintoma: tos
Hora de llegada: 20:49:25
Prioridad: BAJA
--------------------------
--------------------------
Nombre: samuel
Edad: 20
Sintoma: fiebre
Hora de llegada: 20:49:42
Prioridad: BAJA
--------------------------
````
