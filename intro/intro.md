!SLIDE small
# Introducción a GIT #

![Git logo](../2color-lightbg.png) 

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/"><img alt="Licencia Creative Commons" style="border-width:0" src="image/intro/../cc-by-nc-sa-88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/InteractiveResource" property="dct:title" rel="dct:type">Introducción a GIT</span> por <span xmlns:cc="http://creativecommons.org/ns#" property="cc:attributionName">Patricio Keilty</span> se encuentra bajo una Licencia <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/">Creative Commons Atribución-NoComercial-CompartirDerivadasIgual 3.0 Unported</a>.

!SLIDE smaller bullets transition=fade
# Contenido #

* Intro
* Basics
* Branching
* Workflows
* References

!SLIDE smaller bullets incremental
# Qué es git? #
* es un sistema de _código abierto_ de control de versiones 
* diseñado para ser 
** veloz
** simple
** distribuido
** soporte desarrollo no lineal (muchas ramas en paralelo)
** maneje grandes proyectos de manera eficiente (tiempo y espacio) 
* se desarrolló como control de versiones para el kernel del SO Linux en el 2005
* su autor es Linus Torvalds (autor tb del kernel linux)

.notes segunda acepción: un rastreador estúpido/simple de info - [stupid content tracker](http://translate.google.com/#auto|es|you%20are%20a%20git)

!SLIDE smaller
## Taxonomías  SCM ##
### clasificación según almacenamiento: ###
* diffs/deltas
* DAG/snapshots

!SLIDE
## Taxonomías  SCM ##
### Delta vs Snapshot###
![delta](diff-storage-5.png)
![dag](snapshot-storage-5.png)

!SLIDE
## Taxonomías  SCM ##
### Clasificación según arquitectura ###
* local: restringido a la máquina de trabajo
* centralizado: cliente-servidor, única fuente autorizada
* distribuido: red de pares, hay múltiples copias in-sync

!SLIDE transition=fade
## Taxonomías  SCM ##
### Matriz de clasificación ##
![tax](taxonomy-matrix.png)

!SLIDE
## Características ##
* operaciones locales (copia local del repo, no se necesita estar conectado): checkouts, commits, branching, análisis historia
* integridad: cada objeto en la bbdd posee un hash (SHA1 - hex de 40 dígitos - criptográficamente seguro )
* estructura simple de almacenamiento: siempre se escriben datos, no se actualizan
* files 3 estados: commiteado, modificado y en staging (listo para commitear)

!SLIDE transition=fade
## Estados de un file ##
![local](local-states.png)

