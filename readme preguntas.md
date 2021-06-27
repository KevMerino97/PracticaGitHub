*¿Qué comando utilizaste en el paso 11? ¿Por qué?
 R// Utilicé el comando "git reset --hard HEAD~1" para deshacer el último commit y perder los cambios   también en el Working Copy

*¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
 R// Utilice primeramente "git reflog" para poder obtener el identificador del commit que había generado en el paso 10, luego usé "git reset --hard c23aacc" para poder restablecer la infromación tal cual estaba en el commit que había generado en el paso 10 y así, lograr rehacer lo que había deshecho.

*El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
 R// No, porque cuando style absorvió a master, tanto la rama styled como la rama master, están apuntando al mismo commit.

*El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
 R//Si, porque existen commits en ambas ramas del mismo documento en las mismas lineas, provocando un  conflicto en las versiones involucradas. 

*El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
 R//No, master y styled están apuntando al mismo commit y forman una lista.

*¿Qué comando o comandos utilizaste en el paso 25?
 R// Usé primeramente 'git config alias.graph "log --graph --decorate --pretty=oneline" ' para establecer un comando personalizado que me mostrara el grafo, luego ejecuté el comando "git graph" para poder dibujar el grafo desde la consola.

*El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
 R// Si, porque no tendríamos commits inalcanzables que sean utiles si absorvemos a title por fast forward. Tomando en cuenta que en el  paso 19, descartamos el commit de la rama htmlify, no afectaría en nada a la funcionalidad del código. 

*¿Qué comando o comandos utilizaste en el paso 27?
 R// "git reset HEAD~1 para deshacer el merge pero sin perder los cambios del working copy"

*¿Qué comando o comandos utilizaste en el paso 28?
 //R "git reset HEAD git-nuestro.md" para sacar el archivo del stagin area y luego ejecuté "git  checkout -- git-nuestro.md" para poder descartar los cambios.

*¿Qué comando o comandos utilizaste en el paso 29?
 R// "git branch -D title" para poder eliminar dicha rama

*¿Qué comando o comandos utilizaste en el paso 30?
 R// "git reflog" para poder encontrar el commit donde hice el merge y luego ejecuté "git reset --hard  aa7ef68" para poder rehacer nuevamente el merge que había deshecho.

*¿Qué comando o comandos usaste en el paso 32?
 R// "git reflog" para tomar el identificador del commit inicial y "git reset --hard 40272f3" para poder  regresar al commit inicial.

*¿Qué comando o comandos usaste en el punto 33?
 "git reflog" para recuperar el identificador del commit y luego ejecuté " git reset --hard 273cdef" para  regresar nuevamente al estado final donde se le puso título al poema
