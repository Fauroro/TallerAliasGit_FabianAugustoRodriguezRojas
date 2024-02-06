# **Taller Alias Git**

Esta trabajando en un proyecto Git colaborativo con varias ramas y commits. Tu tarea es utilizar el comando git log con algunas opciones específicas para obtener un resumen gráfico de los últimos 5 commits en todas las ramas.

```bash
git config --global alias.ea "log --pretty=format:'%h %s | %d [%an]' --graph -n 5"
```

* **alias.ea -> **genera un alias con la configuracion del log, cuyo nombre es ea
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

```bash
git config --global alias.eb "log --graph --abbrev-commit --decorate --format=format:'%Cred%h%C(reset) %C(yellow)%d%C(reset) %s %Cgreen(%ar)%C(reset)' --all"
```

* **alias.eb -> **genera un alias con la configuracion del log, cuyo nombre es eb
* **--format=format ->** permite especificar la disposicion y el estilo de la salida de registros del commit.
* **%h ->** muestra el hash resumido/corto
* **%s ->** muestra la informacion relacionada con el commit
* **%d ->** muestra las ramas o etiquetas relacionadas con cada commit
* **%ar ->** muestra la fecha relativa del commit
* **--graph ->** muestra el resumen grafico de los commits
* **--abbrev-commit ->**  muestra identificadores de commit abreviados en lugar de mostrar el hash completo.
* **--decorate ->** muestra las referencias (ramas y etiquetas) de cada commit.
* **--all ->** muestra todos los commits
* **%C(color) ->** permite modificar el color de la salida especifica
* **%C(reset) ->** permite restaurar los estilos de la salida a default

## 

Estas trabajas frecuentemente con el comando git log -1 HEAD para obtener detalles sobre el último commit en la rama actual. Sin embargo, encuentras que escribir este comando completo es un poco tedioso. Quieres simplificarlo creando un alias personalizado.

Tu tarea es utilizar el comando git config para crear un alias llamado last que represente el comando git log -1 HEAD.

```bash
git config --global alias.last "log -1 HEAD"
```

* **alias.last -> **genera un alias con la configuracion del log, cuyo nombre es last
* **-1 HEAD ->** muestra los detalles completos sobre el ultimo commit en la rama actual

## 

Imagina que deseas simplificar el proceso de editar la configuración global de Git. Tu tarea es utilizar el comando git config para crear un alias que te permita abrir fácilmente la configuración global en tu editor de texto preferido. Ejecuta el comando para crear un alias llamado ec que cumpla con la especificación dada.

```bash
git config --global alias.ec "config --global -e"
```

* **alias.ec -> **genera un alias con la configuracion requerida, cuyo nombre es ec
* **-e ->** abre la configuracion global de git en el editor de texto preferido

## 

Imagina que estás trabajando en un proyecto Git colaborativo con múltiples colaboradores y ramas. Tu tarea es utilizar el comando git log con opciones específicas para personalizar la salida del historial de commits y resaltar información clave. El resultado de la ejecución del comando se debe ve como el ejemplo siguiente:


```bash
git config --global alias.ed "log --graph --abbrev-commit --decorate --format=format:'%C(yellow)%h%C(reset)%C(red)%d\%C(reset) %s%C(blue)\ [%an]%C(reset)' --all"
```

* **alias.ed -> **genera un alias con la configuracion del log, cuyo nombre es ed
* **--format=format ->** permite especificar la disposicion y el estilo de la salida de registros del commit.
* **%h ->** muestra el hash resumido/corto
* **%s ->** muestra la informacion relacionada con el commit
* **%d ->** muestra las ramas o etiquetas relacionadas con cada commit
* **%an ->** muestra el username de quien realiza el commit
* **--graph ->** muestra el resumen grafico de los commits
* **--abbrev-commit ->**  muestra identificadores de commit abreviados en lugar de mostrar el hash completo.
* **--decorate ->** muestra las referencias (ramas y etiquetas) de cada commit.
* **--all ->** muestra todos los commits
* **%C(color) ->** permite modificar el color de la salida especifica
* **%C(reset) ->** permite restaurar los estilos de la salida a default