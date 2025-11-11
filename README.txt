Como estoy haciendo la primera parte de las prácticas individual, he usado 2 cuentas para simular los 2 usuarios.


Alex -> alexdrin será el alumno 1 Cuyo repositorio local es GIT_IA


Alex2 -> alexdrin773 será el alumno 2 Cuyo repositorio local es GIT_IA2

3

git init

git st

git add .

git commit -m "Inicialización del repositorio con archivos Farmacia"

git remote add origin https://github.com/alexdrin/Git_InterAvan

git remote

git push origin master

Lo que ha ocurrido es que se ha creado en mi repositorio de github la rama master la cual cuadra con los archivos que se encontraban en mi repositorio local en mi carpeta GIT_IA y se ha actualizado el repositorio.

4.

mkdir GIT_IA2

cd GIT_IA2

git clone https://github.com/alexdrin/Git_InterAvan.git

cd Git_InterAvan/

 git switch master

 notepad README.txt

Se ha podido actualizar el repositorio remoto sin problemas ninguno añadiendo este README desde mi repositorio local.

5.

git pull origin master

notepad README.txt

git add README.txt

git commit -m "Actualización de README por el alumno1"

git push origin master