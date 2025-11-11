Como estoy haciendo la primera parte de las prácticas individual, he usado 2 cuentas para simular los 2 usuarios.

Repositorio remoto: https://github.com/alexdrin/Git_InterAvan.git

Alex -> alexdrin será el alumno 1 Cuyo repositorio local es GIT_IA


Alex2 -> alexdrin773 será el alumno 2 Cuyo repositorio local es GIT_IA2

3. Creación e inicialización de un repositorio (Alumno 1)

git init

git st

git add .

git commit -m "Inicialización del repositorio con archivos Farmacia"

git remote add origin https://github.com/alexdrin/Git_InterAvan

git remote

git push origin master

Lo que ha ocurrido es que se ha creado en mi repositorio de github la rama master la cual cuadra con los archivos que se encontraban en mi repositorio local en mi carpeta GIT_IA y se ha actualizado el repositorio.

4.Clonar repositorio (Alumno 2)

mkdir GIT_IA2

cd GIT_IA2

git clone https://github.com/alexdrin/Git_InterAvan.git

cd Git_InterAvan/

 git switch master

 notepad README.txt

Se ha podido actualizar el repositorio remoto sin problemas ninguno añadiendo este README desde mi repositorio local.

5. Actualización README (Alumno 1)

git pull origin master

notepad README.txt

git add README.txt

git commit -m "Actualización de README por el alumno1"

git push origin master

6.Información importante (ambos)

7.Creación de ramas (ambos)

Alumno1:

git checkout -b ramaAlumno1

Alumno2:

git checkout -b ramaAlno2

Para renombrar la rama anterior utilizamos la opción -m de rename/move dentro de la rama que queremos renombrar

git branch -m ramaAlumno2

8. Listar ramas (ambos)
El asterisco encima de la rama muestra la rama en la que te encuentras actualmente trabajando.

9. Modifica el Alumno 1 y Alumno 2 en sus ramas, archivos distintos (ambos)

Alumno1:

nano almacen_cli.java

git add almacen_cli.java

git commit -m "Añadiendo fichero almacen_cli.java"

Alumno2:

git checkout ramaAlumno2

nano cliente.java

git add cliente.java

git commit -m "Añadiendo fichero cliente.java"

10. Ver las diferencias (ambos)
Como no tengo tkdiff instalado al esta en windows, he usado Visual Studio Code para ver las diferencias, estableciendolo como herramienta de diferencias a través del siguiente comando:

git config --global diff.tool "code --diff"

Y para ver las diferencias he usado:

code --diff almacen_cli.java cliente.java

El jefe me ha echado igualmente :(

11. Merge sin conflictos
Comandos usados 
Alumno1:

git checkout master

git pull origin master

git merge ramaAlumno1

git push origin master

Alumno2:

git checkout master

git pull origin master

git merge ramaAlumno2

git push origin master

12. Credenciales

Para no volver a introducir las credenciales he utilizado el siguiente comando:

git config --global credential.helper manager

Alumno 1:

git log --oneline > LogAlumno1.txt

git add.

git commit -m "Añadiendo LogAlumno1"

git pull origin master

git push origin master

Alumno 2:

git log --oneline > LogAlumno2.txt

git add.

git commit -m "Añadiendo LogAlumno2"

git pull origin master

git push origin master

13. Entrega parcial
Para descargar el zip he utilizado directamente la opción de github.

