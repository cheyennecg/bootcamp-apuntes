 # 📅 Día 1 - 06.02.26  
## 🎯 Lo que hemos visto hoy  
### Mañana
- Dinámica: Gartic Phone (sobre distorsión de información)
- Conceptos: ¿Qué es análisis de datos?
- Ejercicio: Palabras en griego (buscar patrones sin contexto)  
### Tarde  
- Git y GitHub: instalación y configuración
- Primeros comandos: clone, status, add, commit, push

## 💡 Lo que he aprendido  
Qué es git y git hub  
Crear un repertorio  
Clonar un repertorio  
Añadir un md y un .gitignore  
## ❓ Dudas que tengo  
¿Cómo borrar archivos md?
¿Se puede mover archivos a otros repertorios?  S 

## 🔗 Recursos útiles  
https://education.github.com/git-cheat-sheet-education.pdf  

## 🔍 Comandos investigados  
### git log --oneline
Te muestra el historial de puntos de guardado (commit) que puedes usar como recurso para saber en que punto te has quedado.  
Siendo el primero en la lista el último guardado.  
Por eso, es importante que los commit sean claros y bien descriptivos sobre el trabajo que has estado haciendo por última vez.  
### git remote -v
Da la info de las URL en las que están conectadas tus proyectos.  

### git branch
Lista todas las ramas creadas y la rama que esta con un * y de color verde es donde estas ubicadada en ese momento.
	main : es la rama principal (el árbol).  

### git pull
Actualiza y descarga toda la info que esta en remoto (Github) a local (El pc que estes usando).  
Es muy útil, porque cuando estais varias personas trabajando en la misma rama te actualiza todo el trabajo o si no estas con tu PC principal puedes editar igualmente.

### .gitignore
No es un comando, es un archivo.
Su función es actuar como una etiqueta de exclusión  "Modo oculto": le indica a Git qué información no debe subir a GitHub.   
Estará en modo oculto en GitHub pero no en git.  
El . al principio indica que es oculto. 


### git add . vs git add archivo  
[git add .] digamos que añade  todo lo que hemos modificado dentro del repositorio donde este aunque tu estes modificando solo un archivo que hay en ese repositorio.  
[git add archivo] añade sólo lo modificado en el archivo que estas trabajando.  
  posteriormente añadir siempre un commit

**Siguiente paso:** Empezar SAT-01 Atlas