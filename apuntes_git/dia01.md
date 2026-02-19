**GIT COMO TRABAJAR**

El sistema de orden del almacén  
*git*: herramienta que instalas para hacer copias de seguridad digamos de todo lo que has estado haciendo en tus códigos.
Almacén  
*git hub* :plataforma del git ( el espacio en la nube) la app donde poder enviar nuestros tabajo y poder usarlos en otros pc o que otros compañeros lo usen.
 
Descargamos Git en nuestro PC y nos presentamos en la terminal

git config global --global user.name "Cheyenne"
git config --global user.name "corrector"
git config -- list es para saber si realmente está modificado el git.
git nit : cable q conecta de remoto a local

Tip:Las carpetas mejor con guiones que espacios

---
GIT
IMPORTANTE ESTAR SIEMPRE EN LA CARPETA O DIRECTORIO QUE QUIERES HACER MODIFICACIONES  

**Flujo típico**
1. Trabajas en tu PC con **Git**
2. Cuando estás contenta con los cambios, los "guardas" dando una pequeña instrucción comimit-m “” (recuerda tener la función autoguardado en code o control+S)
3. Subes esos cambios a **GitHub** (push)
4. Ahora pedirás un PR o mergear a tu main

LA IMPORTANCIA DE LAS RAMAS  
Siempre intentar trabajar en tu rama para no modificar o reventar todo el trabajo global de tu trabajo.
Siempre una rama nueva con cada funcionalidad.
En VS puedes visualizar en qué rama estás abajo a la derecha o git branch en la consola sino siempre te salvará un git status para orientarte dónde estás.
Para crear rama : git branch nombre de la rama ( tener claro siempre en qué carpeta estás que sea el proyecto con el que vas a trabajar o dónde lo vas a alojar)
Si quieres modificar el nombre de la rama git branch -m +“nombre de la rama” +nombre de la rama nueva
Para moverte de rama: git swtich ( esta es la mejor función) o checkout +nombre de la rama que quieres estar
Si quieres eliminar git branch -d + rombre de la rama
Una vez hecho en local le decimos a git que lo suba a remoto con un commit ( git add/git commit/git push (—set-upstream origin +nombre de la rama). Esto último no siempre aparece.
Finalmente si todo está bien revisado haces un PR o lo llevas a main tu con git pull original main  

Funciona a modo “árboles” (main) y cada rama es un trabajo.
Es como si el árbol fuera la sala principal de zoom y las ramas las ramas fueran salas individuales para desarrollar tus trabajos y cuando todo esta okey se mergea al resto del cogido

Anáis :NO CORRIGE RAMAS CON NOMBRE PROPIO; TIENEN QUE HACER ALUSION AL TRABAJO QUE HACES (funcionalidad en la que se esta trabajando)

Si trabajas con más personas en esa rama y quieres que git te dé toda la info actualizada del proyecto hay que hacer siempre un git Pull para traer toda esa info de remoto a local.
Si lo que quieres es una vez que te hayas cerciorado que tu trabajo está bien , un git add+git commit+ git pull.
Como último harás un pull request o mergearlo a tu main.


COSAS QUE PUEDEN PASAR : varias personas estéis modificando el proyecto a la vez y cuando hagas tu push de error…tienes que tenerlo siempre bien actualizado (pull)


PASO PARA ACTUALIZAR TU TRABAJO
Cuando pulsas Ctrl + S, lo único que haces es decirle a Windows: "Escribe estos cambios en el archivo de mi ordenador". Importante antes de enviar la info a github
El color naranja es el aviso de Git diciendo: "Veo que has guardado cosas nuevas en tu local, pero yo aún no las he procesado". Para que lleguen a GitHub, tienes que pasar por estas fases:
git add: Metes el cambio en la "sala de espera" (el archivo sigue naranja pero Git ya lo tiene anotado).
git commit-m :Creas la versión oficial en tu historial local explicando tu cambio resumidamente. Aquí el archivo deja de estar naranja y vuelve al color normal).
git push: Es el único paso que envía la información a GitHub



CREAR GITIGNORE (datos que son comprometidos y no los quieres tener en GitHub)
echo "Thumbs.db" >> .gitignore # Windows
echo "*.tmp" >> .gitignore # Archivos temporales
git add .gitignore
git commit -m "c