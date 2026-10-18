
- **Alumno:** Jhoseen lopez Zambrano
- **Bloque:** B0 — Prerrequisitos
- **Fase / ejercicio:** Fase 0.8
- **Fecha de inicio:** 18/10/2026
- **Fecha de entrega:** 18/10/2026

---

## 🎯 Qué se pedía

* Crear desde cero una bóveda de Obsidian llamada `Boveda_HTML_Casa` y un proyecto web en HTML con su propio repositorio Git local.
* Conectar el proyecto local a un repositorio vacío en GitHub (`sor-web-prestamo-portatiles-casa`) mediante clave SSH.
* Guardar tres versiones con sentido (página inicial, cambio de estado del portátil a mantenimiento, y ampliación con normas, contacto e imagen), ignorando los clips de vídeo locales.
* Realizar un viaje temporal por el historial visitando el primer commit y volver a la rama principal, documentando todo mediante una grabación en vídeo con marcas de tiempo.

## ⌨️ Comandos y pasos importantes

- `git init` — Inicializa un repositorio Git local en la carpeta del proyecto.
- `git remote add origin ...` — Registra la dirección remota del repositorio de GitHub.
- `git add <ruta>` — Prepara los cambios específicos de los archivos para el siguiente commit.
- `git commit -m "mensaje"` — Guarda una nueva versión local identificada con un mensaje descriptivo.
- `git push` — Sube los commits locales acumulados hacia el servidor remoto de GitHub.
- `git check-ignore -v <archivo>` — Comprueba qué regla del archivo `.gitignore` está excluyendo un archivo.
- `git switch --detach <código>` — Permite situarse temporalmente en un commit anterior para consultar el estado antiguo.
- `git switch main` — Regresa a la rama principal del proyecto recuperando el estado actual.

## 🛠️ Qué he hecho

* He comprobado el entorno de trabajo, la identidad global de Git y la autenticación SSH con GitHub antes de empezar (Fase H0).
* He creado la bóveda `Boveda_HTML_Casa`, estructurado las carpetas necesarias e incorporado las reglas en el `.gitignore` para los vídeos (Fase H1-H2).
* He redactado la primera versión del archivo `index.html` con el estado inicial del portátil disponible (Fase H2b).
* He inicializado Git dentro de `01_Proyecto` y vinculado el repositorio remoto de GitHub con `git remote add origin` (Fase H3-H4).
* He registrado la primera versión del proyecto y la he subido a GitHub mediante `git push -u origin main` (Fase H5).
* He modificado el estado del equipo a mantenimiento y guardado la segunda versión (Fase H6).
* He creado las páginas de normas y contacto, incorporado la imagen propia, verificado que los vídeos locales quedan ignorados, preparado los archivos individualmente y guardado la tercera versión (Fase H7).
* He realizado la inspección temporal accediendo al commit inicial con `git switch --detach` y regresado posteriormente a la rama `main` (Fase H7b).
* He grabado el proceso completo en OBS, completado las marcas de tiempo y subido el cierre documental de la bitácora a GitHub (Fase H8).

## 🚩 Qué me ha fallado y cómo lo he resuelto

* **Errores de rutas y nombres de carpeta:** Al crear la estructura inicialmente, escribí el nombre de la carpeta como `Wed` en lugar de `web` y creé el archivo `index.html` fuera de la carpeta `web/`. Tuve que corregir la ruta de los archivos moviéndolos a `web/index.html` y reestructurar las carpetas. 
* **Falta de entregas/commits intermedios:** En un primer intento realicé 2 `push` en lugar de las 3 entregas/commits requeridos en el enunciado para reflejar la evolución del proyecto. * **Solución:** Tuve que repetir la grabación del vídeo desde el principio para corregir la estructura de carpetas, nombrar adecuadamente `web/` y realizar correctamente los 3 commits y sus correspondientes `push` paso a paso según la guía.

## 🤔 Respuestas a las preguntas

1. **¿Por qué `git init` se hizo en `01_Proyecto` y no en la raíz de la bóveda?** Porque la raíz de la bóveda contiene la carpeta `00_Grabaciones` con el vídeo de entrega, por lo que `01_Proyecto` aísla de forma segura exclusivamente los archivos del desarrollo web.
2. **¿Qué mostró `git status` antes de `add`, después de `add` y después de `commit`?** Mostró los archivos sin seguimiento o modificados en rojo, después los preparó en verde, y finalmente dejó el árbol de trabajo limpio tras el commit.
3. **¿Por qué creaste un repositorio de GitHub propio y lo conectaste con `git remote add origin`?** Para mantener un proyecto de casa totalmente independiente del centro y sincronizar el repositorio local con la nube mediante SSH. 
4. **¿Por qué las páginas nuevas aparecen en `git status` pero no en `git diff -- web/index.html`?** Porque `git diff` solo compara las diferencias del archivo indicado (`index.html`), mientras que las páginas nuevas son archivos sin seguimiento (`untracked`) que aparecen en `git status` pero de los cuales no hay historial previo que comparar.
5. **¿Cómo has comprobado que los vídeos existen pero no se van a subir?** Ejecutando `git check-ignore -v web/videos/revision-01.mp4`, lo que indica la regla y línea exacta del archivo `.gitignore` que los excluye. 
6. **¿Qué muestra `git diff --cached --stat` después de preparar los cuatro archivos?** Un resumen estadístico de los archivos que están preparados en el índice (añadidos o modificados) para el próximo commit.
7. **¿Qué cambia al visitar el primer commit y qué recuperas al volver a `main`?** Al visitar el primer commit mediante `git switch --detach`, los archivos retroceden al estado inicial (sin imágenes ni páginas nuevas). Al volver a `main`, se recupera por completo el estado actual ampliado con todo su historial.
8. **¿Por qué esta web necesita historial? ¿Qué aportaría GitHub si otro técnico trabajase contigo?** El historial permite auditar cambios, recuperar versiones anteriores si algo falla y entender la evolución del proyecto. GitHub aportaría un repositorio remoto centralizado para colaborar de forma simultánea, fusionar ramas y revisar código con otros compañeros
9.  **Si mañana corriges una errata en `normas.html`, ¿qué pasos repites y cuáles no?** Se repiten la edición del archivo, `git status`, `git add web/normas.html`, `git commit -m "..."` y `git push`. No se repiten `git init` ni `git remote add origin`, ya que la configuración inicial del repositorio ya está hecha.

## 🔗 Enlaces

- **Vídeo de esta fase:** [B0.P01 · Casa · Préstamo de portátiles](https://youtu.be/ZCkgpzFKf68)
- **Playlist:** [B0.P01 · Casa · Préstamo de portátiles con Git y GitHub](https://youtube.com/playlist?list=PLOKlvpqlPdeI)

## 💭 Dudas / a repasar

que debo practicar mas en escribir o aprenderme los comandos básicos. 