# Proyecto 1 - Permisos y usuarios en Linux

## Descripción

Práctica de laboratorio sobre **gestión y control de permisos en Linux**, orientada a identificar configuraciones incorrectas y aplicar restricciones de acceso para mejorar la seguridad del sistema.

## Objetivos

* Analizar permisos de archivos y directorios.
* Identificar accesos no autorizados.
* Modificar permisos de lectura, escritura y ejecución.
* Trabajar con archivos ocultos.
* Restringir el acceso a directorios.
* Verificar los cambios realizados mediante la terminal.

## Actividades realizadas

### 1. Verificación de archivos y directorios

* Análisis de permisos del directorio `projects`.
* Inspección de archivos visibles y ocultos mediante `ls` y `ls -la`.
* Identificación del archivo oculto `.project_x.txt`.

### 2. Modificación de permisos de archivos

* Identificación de permisos de escritura innecesarios para otros usuarios.
* Modificación de permisos de `project_k.txt`.
* Restricción de permisos del archivo `project_m.txt`.

### 3. Modificación de permisos de un archivo oculto

* Análisis de `.project_x.txt`.
* Eliminación de permisos de escritura.
* Conservación de los permisos de lectura requeridos.

### 4. Modificación de permisos de un directorio

* Análisis de los permisos del directorio `drafts`.
* Identificación del permiso de ejecución otorgado al grupo.
* Eliminación del permiso mediante `chmod g-x`.

## Comandos principales

```bash
ls
ls -la
chmod
cd
```

Ejemplos utilizados durante la práctica:

```bash
chmod o-w project_k.txt
chmod g-x drafts
```

## Conceptos aplicados

* Permisos `r`, `w` y `x`.
* Propietario, grupo y otros usuarios.
* Archivos ocultos.
* Control de acceso.
* Principio de mínimo privilegio.

## Resultado

La práctica permitió aplicar controles de acceso sobre archivos y directorios Linux, eliminando permisos innecesarios y verificando los cambios realizados desde la terminal.

## Documentación completa

La práctica completa, incluyendo las capturas de pantalla y el procedimiento detallado, se encuentra disponible en:

**([Ver documentación completa en PDF](./PORTFOLIO%20EJEMPLAR%20DE%20AGREGAR%20Y%20QUITAR%20PERMISOS..pdf))**
