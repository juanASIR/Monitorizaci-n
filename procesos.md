## **ps -aux** :
```
La opción **a** muestra todos los procesos en ejecución de todos los usuarios del sistema.

La opción **u** proporciona información adicional como el porcentaje de uso de memoria y CPU, el código de estado del proceso y el propietario de los procesos.

La opción **x** lista todos los procesos que no se ejecutan desde el terminal. Un ejemplo perfecto de esto son los daemons, que son procesos relacionados con el sistema que se ejecutan en segundo plano cuando se inicia el sistema.
```

|COMANDO    | USO |
|-------|----------|
|ps -U nombre_usuario|  lista todos los procesos en ejecución de un determinado usuario.  |
|ps -A |  muestra los procesos Linux activos en el formato genérico UNIX |
|ps -T|  imprime los procesos activos que se ejecutan desde el terminal.  |
|ps -C nombre_proceso|  filtra la lista por el nombre del proceso. Además, este comando también muestra todos los procesos hijos del proceso especificado.  |

