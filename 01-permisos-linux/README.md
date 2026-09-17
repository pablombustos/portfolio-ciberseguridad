Proyecto 1 - Permisos y usuarios en Linux
Descripción

En este laboratorio trabajé con permisos de archivos y directorios en Linux. La práctica estuvo enfocada en revisar qué usuarios podían acceder o modificar determinados archivos y después ajustar esos permisos para evitar accesos que no fueran necesarios.

Qué hice

Primero revisé los archivos y directorios del sistema utilizando ls y ls -la. Esto me permitió ver los permisos asignados y también encontrar archivos ocultos, como .project_x.txt.

Después analicé diferentes archivos para detectar permisos de escritura que no eran necesarios para otros usuarios. A partir de eso, modifiqué los permisos de algunos archivos utilizando chmod.

Por ejemplo:

chmod o-w project_k.txt

Con este comando quité el permiso de escritura para otros usuarios sobre project_k.txt.

También trabajé con un archivo oculto y con un directorio llamado drafts. En este último caso, revisé los permisos que tenía asignados al grupo y eliminé el permiso de ejecución utilizando:

chmod g-x drafts

Durante toda la práctica fui verificando los cambios desde la terminal para comprobar que los permisos quedaran como correspondía.

Comandos utilizados

Los principales comandos que utilicé fueron:

ls
ls -la
cd
chmod

Algunos ejemplos de modificaciones realizadas:

chmod o-w project_k.txt
chmod g-x drafts
Conceptos aprendidos

La práctica me permitió trabajar con los permisos de lectura (r), escritura (w) y ejecución (x), además de entender mejor la diferencia entre propietario, grupo y otros usuarios.

También trabajé con archivos ocultos y con el principio de mínimo privilegio, buscando que cada usuario tenga solamente los permisos que necesita.

Resultado

Al finalizar pude identificar permisos que no eran necesarios y modificarlos para restringir el acceso a determinados archivos y directorios. También verifiqué desde la terminal que los cambios se hubieran aplicado correctamente.

Documentación

La práctica completa está documentada en el archivo PDF incluido en este repositorio, donde se pueden ver las capturas de pantalla y el procedimiento realizado paso a paso.

**([Ver documentación completa en PDF](./PORTFOLIO%20EJEMPLAR%20DE%20AGREGAR%20Y%20QUITAR%20PERMISOS..pdf))**
