 1 - He creado un nuevo repositorio en Git y he añadido por defecto el README y el .gitignore
![img.png](img.png)

2 - Creamos un proyecto nuevo con un git repository.
![img_4.png](img_4.png)

3 - Añadimos el repositorio de Github como remoto e intentamos hacer un pull. (Que no funcionará porque ya hemos creado un README y un .gitignore desde GitHub).
![img_5.png](img_5.png)

No podemos hacer un pull porque ya tenemos un .gitignore en local.
Esto ha ocurrido porque hemos marcado la opción de "Create Git repository" ya se ha realizado el git init y se añadió el stage(se ha hecho un git add automatico) pero no commiteamos.

4 - Ahora debemos eliminar el .gitignore para poder proceder con el pull.
![img_6.png](img_6.png)

5 - Y ahora si que podemos hacer el pull.
![img_7.png](img_7.png)

6 - Ahora que ya tenemos descargado lo que estaba en remoto.
Ahora commiteamos el proyecto en local y lo subimos para que quede todo reflejado en remoto.

Añadimos con " Git add ." todo lo que contenga la carpeta.
![img_8.png](img_8.png)

Lo subiremos al repositorio
![img_9.png](img_9.png)

Lo podemos comprobar con "git log --oneline".
![img_10.png](img_10.png)

Y también nos deberá aparecer en nuestra página de git.
![img_11.png](img_11.png)

8 - Eliminamos la rama main en el repositorio de GitHub.

Cambiamos la que esta por defecto a Master y eliminamos main
![img_12.png](img_12.png)

![img_13.png](img_13.png)

9 - Modificamos el proyecto local (con un commit "añadiendi código para probar las propiedades de Java")
![img_14.png](img_14.png)

-Si se te olvida algo de un commit, puedes reahacerlo con el comando "git commit --ammend"
    Este comando nos pediría editar el mensaje del commit, o también podemos utilizar el commando "git commit --ammend --no-edit", que dejaría el mismo mensaje (aunque cambia el hash ya que el contenido y la hora del commit ha cambiado, realmente, es un commit distinto al que teníamos.)

10 - Creamos una nueva rama para corregir un bug:
        Vemos el log con "git log --online" y creamos una nueva rama con "git checkout -b fixBug1"
![img_15.png](img_15.png)

Nueva rama:
![img_16.png](img_16.png)

git checkout sirve para cambiar de commit (en este caso de rama, una rama es un identificador que apunta a un determinado commit (que es el ultimo de su rama ). La opción -b crea una rama nueva (no odríamos hacer checkout a una rama no existente).)

git branch fixBug1 (Crea la rama)
git checkout fixBug1 (Salta a ella)

El error era la class repetida, la eliminamos.
![img_17.png](img_17.png)

11 - Una vez corregido el problema, commiteamos la correccion en la rama y la pusheamos.
![img_18.png](img_18.png)

12 - Hacemos un merge a master con el bug solucionado.
![img_19.png](img_19.png)

13 - Añado el README que estoy haciendo al proyecto este.







