-¿Qué comando utilizaste en el paso 11? ¿Por qué?
Comando utilizado: git reset --hard HEAD~1
Porque se trata de perder los cambios realizados, es decir, volver al commit anterior
de forma que cambie el working copy a dicho estado.

-¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Comandos utilizados: 
git reflog : porque tenía que ver toda la traza de commits al completo para coger
el identificador de interés.
git reset < identificador del commit > para desplazar el puntero hasta dicho commit
(después de este comando he hecho algunos comandos que no hacía falta realizar).
git restore git-nuestro.md : para descartar y volver al estado en el que estaba .

-El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
Comando utilizado: git merge master
No, porque styled contiene los commits de master

-El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Sí, porque no contienen la misma información en las mismas líneas.
Se resuelve el conflicto, se añaden los cambios y se hace el commit correspondiente.

-El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No, porque se trata de un merge de tipo fast forward, de forma que master se 
desplaza hasta donde está el puntero styled para conterner sus commits.

-¿Qué comando o comandos utilizaste en el paso 25?
Comando utilizado: git log --graph
Para pintar el grafo correspondiente al log en dicho punto.

-El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
No, porque no dichas ramas no contienen los mismos commits.

-¿Qué comando o comandos utilizaste en el paso 27?
Comandos utilizados:
git log : para ver la información de los commits.
git reset HEAD~1 : para poder desplazar el puntero al commit anterior.

-¿Qué comando o comandos utilizaste en el paso 28?
Comandos utilizados: 
git status : para comprobar el estado del working copy y el del staging area.
git restore git-nuestro.md : para descartar los cambios del working copy presentes en dicho momento.
git status : para visualizar el resultado del comando anterior.

-¿Qué comando o comandos utilizaste en el paso 29?
Comandos utilizados:
git branch -d title : no generó ningún resultado no estaba mergeada, así que se realizó el siguiente.
git branch -D title : para forzar el borrado de la rama.

-¿Qué comando o comandos utilizaste en el paso 30?
Comandos utilizados: 
git reflog : para obtener el listado de todos los commits realizados y poder obtener
el identificador del commit de interés.
git reset --hard < identificador_del_commit > : para poder desplazar el puntero hasta dicho commit y 
además, modificar el estado del working copy.

-¿Qué comando o comandos usaste en el paso 32?
Comandos utilizados: 
git log : para poder determinar el identificador del commit inicial.
git reset < identificador_del_commit_inicial > : para desplazar el puntero actual hasta dicho commit
sin perder el contenido actual del working copy.

-¿Qué comando o comandos usaste en el punto 33?
Comandos utilizados:
git reflog : para poder visualizar el listado completo de commits realizados y 
obtener el identificador del commit en el que se le añade el título.
git reset --hard < identificador_del_commit_que_añade_título > : para poder desplazar el puntero hasta
dicho commit y además, hacer que el working copy presente dicho contenido.
