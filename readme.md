

# Practica-Git

### **Preguntas y respuestas:**

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
    - Utilicé git reset --hard HEAD~1, porque quería perder los cambios de mi working copy "posicionando head en la posición anterior con ~1".


- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 
    - Utilicé primero git reflog, para ver el rastro que tenía y localizar un commit donde tenia el archivo que había borrado. Despues con git reset me posiciono "head" sobre ese commit y lo recupero con git restore el archivo que había eliminado.


- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué? 
    - Estoy en la rama styled, ejecuto git merge master, no me genero ningun conflicto porque styled nace de la rama main (ha heredado los commit de main hasta ese punto) y al hacer el merge esta todo actializado y no hay cambios.


- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 
    - Si me genero un conflicto, porque los dos archivos han sido editados en dos ramas diferente con diferencias entre sí.


- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 
    - No me genero ningún conflicto porque ha sido fast-foward si el merge puede hacerse fast-foward nunca genera conflictos.


- ¿Qué comando o comandos utilizaste en el paso 25? 
    - Utilicé git log --graph. 

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 
    - Si porque no había conflictos, en title solo añadimos el título pero no hay conflictos en una misma línea en dos ramas distintas.


- ¿Qué comando o comandos utilizaste en el paso 27? 
    - Utilizo git reset HEAD~1 para volver al commit anterior, "sin perder mi working copy" donde no habia hecho el merge de title. 


- ¿Qué comando o comandos utilizaste en el paso 28? 
    - Use git restore del archivo para descartar los cambios. 


- ¿Qué comando o comandos utilizaste en el paso 29? 
    - Use git branch -D title.


- ¿Qué comando o comandos utilizaste en el paso 30? 
    - Use git reflog para localizar donde hice el merge de title, luego me posiciono con git reset "su id", y finalmente hago git restore "archivo".


- ¿Qué comando o comandos usaste en el paso 32? 
    - Use git checkout "id.del commit" para poder volver al momento del historial que quiero, en este momento estoy desconectado del estado de HEAD.


- ¿Qué comando o comandos usaste en el punto 33? 
    - Usando git switch - "si hubiera cambios no quiero guardarlos" volvería donde estaba antes de hacer git checkout "id.del commit", en este caso. Si no fuera el caso repetiría el git checkout "id. del commit" del momento en el que quiera estar, en este caso en el paso 30 "rehacer el merge que hemos deshecho.







