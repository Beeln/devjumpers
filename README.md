**GitHub Ejercitaciñon Final:**

**Pasos:**
Creación del repositorio devjumpers en GitHub.

Luego en git, clono el repositorio con el comando: git clone y el link obtenido del repositorio.

Luego cambio a la carpeta del repositorio creado con el comando: cd devjumpers.

Creo un documento README.md en el repositorio local con el comando: touch README.md

Luego de eso uso el comando: git status para saber que archivos faltan subir a la nube.

Uso el comando: git add . para agregar los archivos a la nube

Despúes uso el comando: commit -m "commit inicial" para comentar el cambio realizado.

Ejecuto el comando: git push para que estos cambios sean subidos al repositorio remoto en la nube.

Ignorar archivos:

Primero creo un fichero llamado privado.txt en el repositorio local con el comando: touch privado.txt

Segundo, creo una carpeta en el mismo repositorio,llamada privada con el comando: mkdir privada

Uso el comando: ls para ver que los archivos estén creados correctamente

Luego el comando: git status, y veo que aparece el fichero privado.txt correctamente en color rojo, ya que no fue subido aún.

Para que el archivo y la carpeta sean ignorados por git, uso el comando: 
touch .gitignore , ya que este archivo de texto,le dice a Git que archivos o carpetas debe ignorar.
Vuelvo a usar el comando: gitstatus y verifico que ya no aparezcan los archivos ignorados.

Ya no aparece el archivo privado.txt en color rojo. 

Añado un fichero llamado 1.txt al repositorio local con el comando: touch 1.txt 

Creo una rama llamada v0.2 con el comando: git branch v0.2

Luego de eso me posiciono en esa rama creada con el comando: git checkout v0.2

Y creo un fichero llamado 2.txt con el comando touch 2.txt 

Luego uso el comando git add .

Y uso el comando commit -m para agregar el comentario del cambio realizado, en este caso fue "Creación de rama nueva y fichero llamado touch 2.txt"

Una vez hecho eso, subo los cambios al repositorio remoto con el comando: git push 

Me posiciono en la rama main con el comando: git checkout main 

Luego hago un merge de la rama v0.2 en la rama master con el siguiente comando: git merge v0.2

En la rama master,agrego "Hola" en el fichero 1.txt y hago commit con los siguientes comandos:
echo "Hola" >1.txt 
Uso git add . nuevamente y luego git status para verificar que falta subir el archivo recién modificado.

Luego el comando: git commit -m "Agregué la palabra Hola al archivo 1.txt" .

Luego cambio a la rama v0.2 con el comando git checkout v0.2 y agrego la palabra "Adios" en el fichero 1.txt con el comando: echo "Adios" >1.txt y uso el comando git add . ,luego git status, y 
hago commit con el comando: git commit -m "Agregué la palabra Adios al fichero 1.txt"

Me posiciono de nuevo en la rama master y hago un merge con la rama v0.2 con el siguiente comando:
git checkout main. Y realizo el merge: git merge v0.2. Luego de esto surge un CONFLICTO que se resuelve en unos pasos más adelante.

Listo las ramas con merge y las ramas sin merge con estos comandos:
git branch --merged y me aparece main ya que se hizo merge a esa rama.
Uso el comando git branch --no-merged y aparece la rama v0.2

Arreglo el conflicto y hago un commit con los siguientes comandos: 
git add .
git commit -m "El conflicto se ha solucionado" 

Para finalizar, Borro la rama v0.2 con el comando:
 git branch -D v0.2
 
Y listo los distintos commits con sus ramas y sus tags con el siguiente comando:
git log --oneline --decorate --all --graph y me figuran así:
*   b17de75 (HEAD -> main, origin/main) El conflicto se ha solucionado
|\
| * e11732a Agregué la palabra Adios al fichero 1.txt
* | 477dfb1 Agregué la palabra Hola al archivo 1.txt
|/
* e39508c (origin/v0.2) Creación de rama nueva y fichero llamado touch 2.txt
* 5a91ff2 commit inicial.

Finalizo con el comando git push , para subir todo al repositorio en la nube.


 NOMBRE  | GITHUB |
| ------------- | ------------- |
| 	Camila Rios  | https://github.com/camilarios01  |
| 	Armando Torres Quintana  | https://github.com/ArmaTQ  |
| 	Geraldine Montufar  | https://github.com/Geraldine1997  |

Colaboradora: Camila Ríos.
