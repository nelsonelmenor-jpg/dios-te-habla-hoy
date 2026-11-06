# Aprende GitHub despacio — La página Dios Te Habla Hoy

## Lo que ya hicimos

1. Creamos la página completa: `index.html`, `README.md` y `COMANDOS.md`.
   La página tiene: versículo del día, Videos, Biblia completa, Libros
   gratis, Devocionales, Temas, Versículos anteriores, **"Oraciones y
   prédicas"** y **"Peticiones"**: formularios que no guardan nada — solo
   arman el texto y lo abren para compartirlo en el grupo de Facebook o
   por WhatsApp. Los comentarios y las prédicas (texto, audio o video)
   se publican como publicaciones del grupo.
2. Falta un paso que solo se puede hacer desde la cuenta de Nelson en el navegador:
   crear el repositorio público **dios-te-habla-hoy** en https://github.com/new
   (nombre: `dios-te-habla-hoy`, descripción: "Un versículo de la Biblia y una
   historia corta cada día, para empezar tu día con fe. Dios te habla hoy.",
   público, sin README inicial). La aplicación de GitHub que usa Muse no puede
   crear repositorios nuevos: dio error 403 dos veces. Por eso este paso es en
   el navegador.

## Los comandos, uno por uno (para aprender despacio)

Cuando el repositorio ya exista, estos son los comandos que se usan.
Cada comando hace una sola cosa:

```bash
# 1. Ver quién soy en GitHub
gh auth status

# 2. Copiar el repositorio a mi computadora (clonar)
git clone https://github.com/nelsonelmenor-jpg/dios-te-habla-hoy.git

# 3. Entrar a la carpeta del proyecto
cd dios-te-habla-hoy

# 4. Ver qué archivos hay
ls

# 5. Ver qué cambió
git status

# 6. Guardar los cambios (los archivos nuevos y actualizados)
git add index.html README.md COMANDOS.md

# 7. Confirmar los cambios con un mensaje
git commit -m "Agrego la página Dios Te Habla Hoy"

# 8. Subir los cambios a GitHub
git push
```

## Activar GitHub Pages (para que la página se vea en internet)

En el navegador, dentro del repositorio:
**Settings → Pages → Source: Deploy from a branch → Branch: main → Save.**

La página quedará en:
https://nelsonelmenor-jpg.github.io/dios-te-habla-hoy/

## Actualizar el versículo cada día

1. Abre `index.html` y cambia la fecha, el versículo y la historia.
2. Guarda.
3. Repite solo estos tres comandos:

```bash
git add index.html
git commit -m "Versículo del día"
git push
```

En unos minutos la página ya muestra el versículo nuevo.
