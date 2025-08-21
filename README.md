# 🚀 Hackatón 0 – CS2031  

¡Bienvenidos chicos! 🎉  
Desde el curso **CS2031** les damos una cordial bienvenida e inicio de ciclo **2025-2**. Sabemos que están llenos de energía y ansiosos por comenzar a colaborar en equipo.  


## 🤔 ¿Qué es la Hackatón 0?  
Esta es una **primera muestra** del concepto de *hackatones*: un tipo de actividad calificada que, al inicio, muchos podrían odiar 😅…  
Pero al final se darán cuenta de que es la que más los prepara para la **industria real**.  

👉 Sentarse en equipo, colaborar bajo presión y resolver un problema en poco tiempo es una de las habilidades más valoradas y buscadas en el mundo laboral.  



## 👥 Trabajo en equipo  
Antes que nada, escoge bien a tu equipo.  
No solo se trata de divertirse mientras trabajan, sino de **complementarse**:  

- Habrá quienes sean buenos organizando 🗂️  
- Otros que lideren 🧭  
- Y otros que ejecuten rápido ⚡  
- Pero también quienes sean buenos en la parte técnica 💻  

Esta hackatón es **trabajo en equipo + Git + GitHub**.  
Ni siquiera es necesario programar. El reto está en **la comunicación** 🗣️, en cómo coordinan y se reparten las tareas. Poco a poco irán desarrollando esta habilidad clave.  

## 😢 ¿Qué pasa si no viste el video de Git y GitHub?

Que Bellido se apiade de ti 🙏… ¡nah, es broma! 😅 No te preocupes. Si aún no lo revisaste, aquí está el hermoso video preparado con mucho cariño por tus TAs favoritos, Mauricio y tu humilde servidor Gabriel: [👉 Video de introducción a Git y GitHub](https://www.youtube.com/watch?v=8CmZysIzcbc)

Eso sí, ⚠️ es crucial que lo aprendas cuanto antes. Git y GitHub serán herramientas que usarás en todo el curso y en tu vida profesional:

* Para colaborar con código 👩‍💻👨‍💻
* Para subir tareas y proyectos 📂
* Incluso para construir tu propio portafolio de trabajo 💼

Si no lo ves ahora, probablemente sufras un poco en esta hackatón 🔥… ¡pero tranquilo! Al menos estás en equipo, así que siempre puedes pedir ayuda a tus compañeros para ir avanzando. Recuerda: la unión hace la fuerza 💪

## 📜 El reto

Resulta que un TA (no diremos nombre 🤫) estuvo moviendo los archivos, alterando el git y **rompió el proyecto de la página web**.  

🎯 **Tu objetivo:** corregir los errores y restaurar el proyecto a su estado funcional, de modo que el equipo pueda tener lista su **primera página web** y finalmente **desplegarla en GitHub Pages**. 🚀  



## 👑 Organización del equipo
- Elijan un **líder de equipo**.  
- El líder abre un issue llamado **“Checklist del equipo”**.  
- Cada integrante trabaja en **su propia rama individual** (`feat/member-nombre`) y abre un PR.  
- Habrá **conflictos intencionales** en el código que deberán resolver colaborativamente.  


## ✅ Pasos principales

1. **Seleccionar un líder de equipo**  
   - Encargado de crear issues, coordinar y supervisar el progreso.  

2. **Checklist del equipo (issues a crear por el líder):**  

   - **#1 Nombres (PR por persona)**  
     - Editar la lista `<ul id="contributors">` en `index.html`.  
     - Agregar `<li>Su Nombre</li>` en su rama.  
     - **Conflicto esperado:** varios editan la misma línea → deberán resolverlo conservando todos los nombres.  

   - **#2 CSS separado (1 PR)**  
     - En `main` el CSS es un **archivo monolítico azul**.  
     - En `clean-css` ya está modularizado con imports y un `h1 { color: red; }`.  
     - **Conflicto esperado:** azul vs rojo en el `h1`.  

   - **#3 Navbar (1 PR)**  
     - En `main` los anchors están rotos (`#integrantes`).  
     - En `navbar-fix` los restauraron a `#team`, pero además cambiaron el título del hero.  
     - **Conflicto esperado:** decidir si queda el título original o el nuevo.  

   - **Publicado en Pages**  
     - Hacer merge limpio hacia `main`.  
     - Activar GitHub Pages desde `main`.  
     - Validar que el sitio funcione.  

## ⚡ Ejemplo de conflicto

Cuando dos ramas modifican la misma parte del archivo, Git lo marca así:

```html
<h1 class="hero__title">
<<<<<<< HEAD
  Welcome to Git & GitHub
=======
  Welcome to Git & GitHub – CS2031
>>>>>>> navbar-fix
</h1>
````

👉 El equipo debe **resolver manualmente**, quitando los marcadores y dejando una versión consensuada:

```html
<h1 class="hero__title">
  Welcome to Git & GitHub – CS2031
</h1>
```

Espero les sirva esta guía para abordar el reto. Con cariño, su TA a distancia Gabriel. 😊