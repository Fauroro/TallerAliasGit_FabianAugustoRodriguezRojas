# **Taller Alias Git**

Esta trabajando en un proyecto Git colaborativo con varias ramas y commits. Tu tarea es utilizar el comando git log con algunas opciones específicas para obtener un resumen gráfico de los últimos 5 commits en todas las ramas.

```bash
$ git config --global alias.e1 "log --pretty=format:'%h %s | %d [%an]' --graph -n 5"
```

* **alias.e1 -> **genera un alias con la configuracion del log, vuyo nombre es e1
* **--pretty=format ->** permite especificar la disposicion de la salida de registros del commit.
* **%h ->** muestra el hash resumido/corto
* **%s ->** muestra la informacion relacionada con el commit
* **%d ->** muestra las ramas o etiquetas relacionadas con cada commit
* **%an ->** muestra el username de quien realiza el commit
* **--graph ->** muestra el resumen grafico de los commits
* **-n 5 ->** selecciona unicamente los ultimos 5 commits realizados

## 

Esta trabajando en un proyecto Git colaborativo y necesitas obtener una visión gráfica y detallada del historial de commits. Tu tarea es utilizar el comando git log con opciones específicas para personalizar el formato y presentación de la salida. La salida debe tener las siguientes especificaciones:

- Muestra una representación gráfica del historial de commits
- Muestra el hash corto del commit en color rojo
- Muestra las referencias (ramas o tags) en las que está involucrado el commit en color amarillo
- Muestra el mensaje del commit.
- Muestra la fecha relativa del commit en color verde.
- Muestra el hash del commit como un identificador abreviado.
  - Muestra las fechas de los commits de forma relativa





Estas trabajas frecuentemente con el comando git log -1 HEAD para obtener detalles sobre el último commit en la rama actual. Sin embargo, encuentras que escribir este comando completo es un poco tedioso. Quieres simplificarlo creando un alias personalizado.

Tu tarea es utilizar el comando git config para crear un alias llamado last que represente el comando git log -1 HEAD.





Imagina que deseas simplificar el proceso de editar la configuración global de Git. Tu tarea es utilizar el comando git config para crear un alias que te permita abrir fácilmente la configuración global en tu editor de texto preferido. Ejecuta el comando para crear un alias llamado ec que cumpla con la especificación dada.





Imagina que estás trabajando en un proyecto Git colaborativo con múltiples colaboradores y ramas. Tu tarea es utilizar el comando git log con opciones específicas para personalizar la salida del historial de commits y resaltar información clave. El resultado de la ejecución del comando se debe ve como el ejemplo siguiente: