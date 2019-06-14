## Respuestas a cuestiones práctica 

11

`git reset --hard HEAD~1`
Porque este comando deshace tanto el commit como los cambios hechos en el working directory gracias al comando --hard.

12

Primero `git reflog`, así podemos ver exactamente dónde estamos, en que commit nos encontramos antes de hacer el reset y que 
cambios ha habido.
Gracias a los comentarios de los commit o la tag(si hemos puesto alguna)
sabemos que ID de commit estamos buscando para recuperar el commit, en este caso el 040ea67.
Con `git reset --hard 040ea67`  recuperaremos el commit y los cambios que habia hecho en el working directory. Comprobamos con 
`git log` y con `cat git-nuestro.md` y vemos que todo está correcto.

13

`Git merge master`, sin conflictos, ningún cambio en parent

19

Sin conflicto

21

Sin conflicto

25

`git log --grap --decorate --oneline`

26

`git merge --no-ff title`

Podría ser fast forwart, aunque entonces no creariamos un nuevo commit y master absorveria directamente a title.
27

`git reset HEAD~1`

28

`git checkout --git-nuestro.md`

29

`git branch -D title`

30

`git reflog`, buscamos ID del merge hecho anteriormente
`git reset --hard <id merge>`

32

`git reflog`
`git reset --hard <id primer commit>`

33

`git reset --hard <id del paso 30>`



