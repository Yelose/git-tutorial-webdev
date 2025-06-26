# 📌 Resumen de comandos de Git y GitHub

Este documento recopila **todos los comandos** vistos durante el curso para que puedas consultarlos fácilmente.

---

## 🔧 Configuración inicial

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
git config --list
```

---

## 📁 Iniciar un repositorio

```bash
git init
```

---

## 📄 Añadir archivos y hacer commits

```bash
git status
git add .
git add nombre-archivo
git commit -m "Mensaje del commit"
```

---

## 📜 Ver historial y cambios

```bash
git log              # Ver el historial de commits
git diff             # Ver los cambios sin añadir
git diff --staged    # Ver los cambios añadidos (con git add)
```

---

## 🌐 Conectar con GitHub

```bash
git remote add origin https://github.com/usuario/repositorio.git
git branch -M main
git push -u origin main
git pull origin main
```

---

## 🌱 Trabajar con ramas

```bash
git branch                  # Ver ramas
git branch nueva-rama       # Crear rama
git switch nombre-rama      # Cambiar de rama (Git 2.23+)
git checkout nombre-rama    # Cambiar de rama (versión antigua)
git checkout -b nueva-rama  # Crear y cambiar de rama
git merge nombre-rama       # Fusionar rama a main
git branch -d nombre-rama   # Borrar rama local
```

---

## 🤝 Clonar y colaborar

```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 🚀 Publicar una web con GitHub Pages

> No se hace por terminal. Sigue estos pasos en la web:

1. Entra en tu repositorio.
2. Ve a **Settings > Pages**.
3. Selecciona la rama `main` y la carpeta `/root`.
4. Guarda y espera unos segundos.
5. Visita el enlace que aparece para ver tu página.

---

## 🧠 Consejos útiles

* Usa `git status` constantemente para no perderte.
* Haz commits con frecuencia y con mensajes claros.
* Si no recuerdas un comando, escribe `git help` o búscalo aquí.

---

🧾 **Este resumen es tu guía de bolsillo para empezar a trabajar con Git y GitHub como un/a profesional.**

---

# 🧪 Comandos útiles que aún no hemos visto (investigación personal)

Estos comandos no se han cubierto en el curso, pero son muy usados en entornos profesionales. Puedes investigar cómo y cuándo se usan:

### 📌 Comandos para investigar

| Comando                     | ¿Para qué sirve? |
|----------------------------|------------------|
| `git stash`                | Guarda cambios no comprometidos para recuperarlos más tarde. Ideal si necesitas cambiar de rama sin perder lo que estás haciendo. |
| `git reset`                | Revierte cambios en el área de preparación o en el historial de commits. (¡Cuidado! Puede borrar cambios si no se usa bien). |
| `git revert`               | Crea un nuevo commit que deshace un commit anterior (sin borrar historial). |
| `git rebase`               | Reorganiza el historial de commits para dejarlo más limpio. Muy útil pero avanzado. |
| `git log --oneline`        | Muestra el historial de commits en una línea por commit, ideal para ver todo de forma rápida. |
| `git show`                 | Muestra los detalles de un commit específico. |
| `git diff nombre-rama`     | Compara tu rama con otra. Útil para ver qué cambiará antes de hacer un merge. |
| `git cherry-pick`          | Copia un commit concreto de otra rama sin traer todo lo demás. |
| `git tag`                  | Marca una versión específica del proyecto, útil para releases (v1.0, etc.). |
| `git fetch`                | Descarga cambios del repositorio remoto sin mezclarlos aún. Útil para ver qué hay de nuevo antes de hacer `pull`. |
| `git remote -v`            | Muestra las URLs conectadas al repositorio local. |

---

🔍 Puedes buscar cada uno en Google o probarlo en un repositorio de prueba:

> Por ejemplo:  
> `git stash tutorial`  
> `git reset vs revert`  
> `git rebase explicado`

---

🧠 Aprender estos comandos te permitirá trabajar en proyectos más grandes y con equipos de forma profesional.

¡Claro! Aquí tienes una sección final para añadir al archivo `resumen/README.md` bajo el título **"🧑‍🏫 Recomendación personal"**, tal como lo pedirías a tu alumnado en clase:

---


## 🧑‍🏫 Recomendación personal

Aunque Git tiene comandos muy potentes como `git checkout`, te recomiendo lo siguiente:

- Usa `git switch` para **cambiar de ramas**.
- Usa `git restore` para **deshacer cambios en archivos**.

### ¿Por qué?

Porque `git checkout` puede causar errores si no se usa bien. Por ejemplo:

- Si tienes cambios sin guardar (archivos que han sido modificados en tu editor, pero todavía no se han añadido con git add y por tanto no están incluídos en ningún commit) y haces `git checkout otra-rama`, Git puede **intentar hacer un merge automático sin avisar**.
- También puedes sobrescribir archivos sin darte cuenta.

🧠 **En resumen**:
> ✅ Usa `switch` para moverte entre ramas, y  
> ✅ Usa `restore` para volver atrás en un archivo.  
> ❌ Evita `checkout` si no tienes claro lo que hace.

Esto te ahorrará problemas en proyectos reales o en equipo.
