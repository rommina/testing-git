# testing-git
Test respository

## Como clonar este repositorio.

Abre una terminal, dirigete a la carpeta donde queres clonar este repositorio.

´git clone direccion_del_repositorio´

la direccion del repo se obtiene en github, en el boton "CODE" y se copia la direccion en HTTPS.

´git clone https://github.com/MarianaArrobaMedina/testing-git.git´

Nos creara una carpeta con el nombre del proyecto, en nuestro caso testing-git

## Agregando cambios

Abrir su proyecto en VSCode crear un archivo.

## Chqueando el estado del repositorio

´git status´

Nos mostrara el archivo que hemos creado como un cambio no "stageado" (PREPARADO):

´git add nombre_de_archivo´

nos permite llevar el archivo a un estado previo a ser "commiteado" (LISTO):

si repetimos ´git status´, veremos que el archivo ahora esta en verde listo para ser enviado al origen (PUSH) o para quedar en nuestra rama local.

Notaran que git nos da la posibilidad de remover el archivo del commit con el comando "git restore nombre_del_archivo"

## Hacer commit de un archivo

´git commit´ (Abrira un editor que mostrara los archivos a ser commiteados (puede ser mas de uno) y les permitira ingrasar un mensaje mas completo e util para el historial, si el editor es "nano" se guarda con Ctrl+S, se sale con Ctrl+X)

o 

´git commit -m "Mensaje del commit"´

PARA LEERE MAS TARDE: https://tomasdelvechio.github.io/old/440/
Estandarizacion de mensajes de commmit.

## Chequear el historial de commits

Una vez que se hace el commit podemos chequear el historial con:

´git log´

Nos permite saber si tenemos commits que no hemos enviado al repositorio origen.

En VSCode pueden utilizar la extension "git history" y si lo queiren ver graficamente pueden instalarse "git graph"

## Hacer push de los cambios (enviar los commits al repositorio origen)

´git push´ (conveniente chequear con git status que estas en la rama correcta)

o

´git push origin master´ (envia los cambios a la rama master)

Si todo salio bien podras ver tus cambios en el repo en GITHUB.

## Hacer un pull de master (Obtener los cambios hechos por otros que aun no tenemos en local = syncronizar la rama master local con la rama master del origen)

´git pull´ (conveniente chequear con git status que estas en la rama correcta)

o

´git pull origin master´
