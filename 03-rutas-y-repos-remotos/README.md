# 03 - Rutas y Repos Remotos en GitHub

Ahora que ya tienes tu repositorio local creado, vamos a enlazarlo con un repositorio en GitHub para poder guardar tu proyecto en la nube y acceder a él desde cualquier sitio.

---

## 🐙 1. Crear una cuenta en GitHub (si no la tienes)

1. Ve a [https://github.com](https://github.com)
2. Haz clic en **Sign up** y sigue los pasos.
3. Verifica tu correo electrónico.

---

## 📦 2. Crear un repositorio en GitHub

1. Una vez dentro de tu cuenta, haz clic en el botón verde **"New"** (o "+" arriba a la derecha).
2. Escribe un nombre para tu repositorio (por ejemplo: `mi-primer-repo`)
3. Elige la opción **"Public"** o **"Private"** según prefieras.
4. **No marques** la opción de "Add a README" (ya lo tienes tú localmente).
5. Haz clic en **"Create repository"**

Verás una página con instrucciones, como esta:

```bash
git remote add origin https://github.com/tuusuario/mi-primer-repo.git
git branch -M main
git push -u origin main
```

---

## 🔗 3. Enlazar tu proyecto local con GitHub

Desde la terminal de tu carpeta local (en VS Code o en tu terminal habitual):

```bash
git remote add origin https://github.com/TU-USUARIO/mi-primer-repo.git
```

(Sustituye la URL por la que te da GitHub)

Asegúrate de que tu rama se llama `main`:

```bash
git branch -M main
```

Sube tu proyecto a GitHub:

```bash
git push -u origin main
```

---

## 🚨 ¿Qué pasa si falla el push?

Es posible que veas algo como:

```
fatal: The current branch main has no upstream branch.
```

Eso es porque necesitas decirle a Git que quieres subir la rama actual con este comando (ya lo hiciste si copiaste el anterior):

```bash
git push -u origin main
```

---

## 🧭 Comandos usados en esta lección

```bash
git remote add origin URL     # Enlaza tu repositorio local con GitHub
git branch -M main            # Asegura que tu rama principal se llama 'main'
git push -u origin main       # Sube tu código a GitHub por primera vez
```

---

## 📍 Puedes comprobar que todo ha ido bien si...

* Refrescas tu repositorio en GitHub y ves tu archivo `index.html`.
* Ya puedes compartir tu proyecto con tu profesora o compañeros.

---

👉 Siguiente lección: [04 - Ramas y colaboración](https://github.com/Yelose/git-tutorial-webdev/blob/main/04-ramas-y-colaboracion/README.md)


