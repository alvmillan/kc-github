### ¿Qué comando utilizaste en el paso 11? ¿Por qué?

>`git reset --hard HEAD~1`

> Este comando permite volver atrás 1 posición en la lista de cambios. Podriamos volver atrás `n` posiciones usando `HEAD~{n}`. <br>
> Al no querer conservar los cambios en el staging area le ponemos `--hard` para que haga un cambio completo.

### ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

>`git reflog` <br>
>`git reset --hard b3a6021`

> El comando `reflog` permite ver la lista de todos los commits con sus identificadores. <br>
> Con este comando podemos ir a cualquier posicion en la lista de cambios. En este caso lo que estamos haciendo es identificar el commit anterior por su id único `b3a6021` para así volver y "rehacer" el commit (un commit es permanente y no puede rehacerse porque no puede eliminarse, lo que verdaderamente estamos haciendo es volver a él por su id). <br>

### El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

> Lo que hay es un aviso `already up to date` por parte de git diciendo que la rama `styled` ya contiene toda la funcionalidad de `master` y no mergea porque no tiene nada que mergear.


### El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

> Sí, hay un conflicto entre las líneas con formato Markdown y las líneas con formato HTML. El fichero git-nuestro.md guarda una copia con ambas versiones en distintas líneas y tu debes decidir con cual te quedas en cada caso. <br>

> Desde Visual Studio Code hay una especie de helper que te permite comparar y aceptar cambios. Una vez esté todo solucionado hay que guardar los cambios añadiendolos al staging y haciendo commit.

### El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

>No hay ningún tipo de conflicto ya que simplemente la rama `master` absorbe los estilos markdown de `styled` y se los hace suyos.

### ¿Qué comando o comandos utilizaste en el paso 25?

> `git log --graph`

### El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

> Si, ya que moviendo el puntero master a la posición del puntero title, tendría accesibilidad a los commits de title.

### ¿Qué comando o comandos utilizaste en el paso 27?

> `git reset HEAD~1`

> Vuelve una posición atrás pero no deshace cambios en el staging area porque no es `--hard`.

### ¿Qué comando o comandos utilizaste en el paso 28?

> `git checkout -- git-nuestro.md`

> Este comando sirve para quitar cosas del staging area. En este caso el fichero git-nuestro.md

### ¿Qué comando o comandos utilizaste en el paso 29?

> `git branch` <br>
> `git branch -D title`

> Primero miro la lista de ramas y despues con el comando `-D` elimino la que deseo.

### ¿Qué comando o comandos utilizaste en el paso 30?

> `git reflog` <br>
> `git reset --hard 237d332`

> Miro el commit exacto al que me interesa ir con reflog y accedo a él con reset.

### ¿Qué comando o comandos usaste en él paso 32?

> `git reflog` <br>
> `git reset --hard b5459e3`

> Miro el commit exacto al que me interesa ir con reflog y accedo a él con reset.
### ¿Qué comando o comandos usaste en el punto 33?

> `git reflog` <br>
> `git reset --hard 237d332`

> Miro el commit exacto al que me interesa ir con reflog y accedo a él con reset.