@uthor : Isabel Calzadilla


# Práctica del curso de git, gitHub y Sourcetree

Información de contacto del profesor:
</br>
Alberto Casero
</br>
acasero@agbotraining.com
</br>
Skype: kas.appeal
</br>
Twitter: @KasAppeal


## Ejercicio 1   


Se deberá crear un repositorio y realizar una serie de operaciones desde la consola de
comandos sobre el mismo para posteriormente subir el repositorio a Github.
Se deberá entregar a través del formulario de prácticas indicando la URL del repositorio. En el
repositorio, deberá existir un archivo readme.md con las respuestas a las siguientes preguntas:




## ¿Qué comando utilizaste en el paso 11? ¿Por qué?

![imagen](https://user-images.githubusercontent.com/36207623/203640265-b2dc8832-e64b-4232-b39d-753b4ff3bb34.png)


El comando que usé fue el:
                        
                                    ' git reset --hard HEAD~1'

      
Ésto motivado a que sólo necesitaba retraer el puntero una posición para volver al estado original y deshacer los cambios.



## ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?


El comando que usé fue :

                                    'git reflog'
                                    
![imagen](https://user-images.githubusercontent.com/36207623/203641324-6e8dd463-1cea-4bd4-be6a-e969b1c8feeb.png)

Ésto para lograr dar con el Hash específico del commit que me interesaba, y luego posicionar el puntero sobre el mismo con el comando :

                                    'git reset --hard 99514cb'
                                    
 Con el mismo, se restauró el commit.
 
 

## El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?


No, en el caso del Merge de la rama 'main' a 'styled' no causó conflicto alguno ya que se mantuvieron los cambios.


## El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?


En éste caso sí causó conflictos en la rama al intentar 'styled' absorber a 'htmlify' ya que las mismas contenian versiones distintas en las mismas líneas, lo resolví manteniendo la versión de 'styled' como indicaba el enunciado.


## El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No causó conflicto, previamente en el Merge que sí lo causó se mantuvo la versión de 'styled' que a su vez apuntaba a los commits de 'main' por lo cuál, mantenía su versión, fue un FastForward en toda regla.


## ¿Qué comando o comandos utilizaste en el paso 25?


La muestra del diagrama por cónsola se ejecutó mediante el siguiente comando :


                                    '$ git log --graph'
                                    
y dió como resultado el siguiente grafo :


![imagen](https://user-images.githubusercontent.com/36207623/203643581-28a8b5c0-ebc4-47cd-9da1-da0127a62c05.png)

                                    
## El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?


El merge sí puede ser un FastForward ya que contienen básicamente el mismo commit y sólo habría que subir el HEAD al escalón a apuntar.

Al hacer uso del comando ' --no-ff '  lo forzamos, de hecho, para que no sea FastForward explícitamente.


## ¿Qué comando o comandos utilizaste en el paso 27?

El comando usado fue :

                              ' $ git reset HEAD~1 '
                              
Lo usamos para retraer el puntero una posición y retornar todo hasta ese punto.                              

![imagen](https://user-images.githubusercontent.com/36207623/203645965-5db49f3f-ae8f-4c72-b477-10d194845d28.png)


## ¿Qué comando o comandos utilizaste en el paso 28?

El comando usado fue :
                              ' $ git reset --hard '
                              
                              
## ¿Qué comando o comandos utilizaste en el paso 29?

El comando usado fue :
                              ' $ git branch -D title '
                              
                              
Con la '-D' forzamos a eliminar la rama que definamos, el comando puede usarse en mayúsculas y minúsculas, aunque para evitar contrariedades es recomendable sea en mayúsculas pues es una manera 'HARD' de hacerlo.                              
                              
![imagen](https://user-images.githubusercontent.com/36207623/203646489-c3d7c655-742b-425d-80d6-f38a3b4ee2a5.png)


## ¿Qué comando o comandos utilizaste en el paso 30?

Inicialmente debemos de ubicar el Hash que identificó ese cambio en GIT, lo realizamos con

            Comando   :     ' git reflog '
           

Luego de ubicar nuestro Hash, sencillamente llamamos al comando :

                            ' git reset --hard 0a0fc88  '                                    


## ¿Qué comando o comandos usaste en el paso 32?

Debido a que se nos demanda el commit inicial, debemos de hacer uso del Log para llegar hasta él.

            Comando   :       'git log'
            
            
 Con el mismo, se nos muestra el orden cronológico de todos los commits, luego de ubicarlo, sencillamente nos hacemos con el Hash y llamamos al comando
 
                              '$ git reset --hard 345466e304324f87d093c11d5c28424dc35ff3cb '
                              
 Con lo cuál forzamos a sobreescribir hasta el primer commit.
 
 
 ![imagen](https://user-images.githubusercontent.com/36207623/203648360-0abb81eb-b995-49cf-b2a1-81f80bb19ebf.png)

 
## ¿Qué comando o comandos usaste en el punto 33?


Para restituir todo hasta el punto final, sencillamente usamos el reflog para ubicar el último cambio, en éste caso el merge, tomamos el Hash de dicho paso y hacemos uso del comando :

                              ' $ git reset --hard 0a0fc88 '




# Instrucciones a seguir :

Los pasos a ejecutar son los siguientes (los pasos en negrita indican que hay una pregunta
asociada):


 1) Crear un repositorio
 2) Crear un archivo git-nuestro.md con el contenido:

# Git nuestro

Git nuestro que estas en los repos
Comprimidos sean tus commits
Venga a nosotros tu log
En el local como en el remote
Danos hoy nuestro pull de cada día
Perdona nuestros conflictos
Como también perdonamos los de otros geeks
No nos dejes caer en detached HEAD
y líbranos de SVN
git commit --amend


 3) Añadir git-nuestro.md al staging area
 4) Mover lo que hay en el staging area al repositorio
 5) Crear una rama llamada “styled”
 6) Listar las ramas que hay en el repositorio
 7) Moverse a la rama “styled”
 8) Comprobar que se está en la rama correcta
 9) Modificar en el archivo git-nuestro.md:

*Git* nuestro que estás en los repos
Comprimidos sean tus *commits*
Venga a nosotros tu *log*
En el local como en el *remote*
Danos hoy nuestro *pull* de cada día
Perdona nuestros *conflictos*
Como también perdonamos los de otros geeks
No nos dejes caer en *detached HEAD*
y líbranos de *SVN*
`git commit --amend`

 10) Añadir los cambios al staging area y luego pasarlos al repositorio
 11) Deshacer el último commit (perdiendo los cambios realizados en el working copy)
 12) Rehacer el último commit (el que acabamos de deshacer)
 13) Hacer un merge con ‘master’ (styled absorbe a master)
 14) Volver a la rama master
 15) Crear una nueva rama llamada “htmlify”
 16) Cambiar a la rama htmlify
 17) Modificar en el archivo git-nuestro.md:

<p><em>Git</em> nuestro que estas en los repos<br />
Comprimidos sean tus <em>commits</em><br />
Venga a nosotros tu <em>log</em><br />
En el local como en el <em>remote</em><br />
Danos hoy nuestro <em>pull</em> de cada día<br />
Perdona nuestros <em>conflictos</em><br />
Como también perdonamos los de otros geeks<br />
No nos dejes caer en <em>detached HEAD</em><br />
y líbranos de <em>SVN</em><br />
<code>git commit --amend</code></p>

 18) Hacer un commit
 19) Hacer un merge de “htmlify” en “styled” (styled absorbe a htmlify)
 20) Si hay conflictos, deberemos resolverlos quedándonos con el contenido de la rama “styled”.
 21) Desde “master”, hacer un merge con “styled”
 22) Crear una rama “title” y cambiarse a esa rama
 23) Añadir un título (a tu gusto) al archivo git-nuestro.md y hacer un commit.
 24) Volver a la rama master
 25) Dibujar el diagrama
 26) Hacer un merge “no fast-forward” de “title” en “master” (master absorbe a title)
 27) Deshacer el merge (sin perder los cambios del working copy)
 28) Descartar los cambios
 29) Eliminar la rama “title”
 30) Rehacer el merge que hemos deshecho
 31) Volver a master y eliminar el resto de ramas
 32) Volver al commit inicial cuando se creó el poema
 33) Volver al estado final, cuando pusimos título al poema
 34) Crear los siguientes tags:

      inicial: en el primer commit
      styled: modificación del paso 10
      htmlify: modificación del paso 17-18
      title: modificación del paso 30

 35) Ir al tag htmlify
