# 02 - Comandos Básicos de Git

Ahora que tienes Git instalado y configurado, vamos a crear tu primer repositorio y aprender los comandos más importantes para guardar tus cambios y trabajar con versiones de tu proyecto web.

---

## 📁 1. Crea tu carpeta de proyecto

### 🔸 Opción A: Desde el explorador de archivos (sin consola)

1. Abre tu carpeta habitual de documentos o escritorio.
2. Crea una nueva carpeta y ponle un nombre, por ejemplo: `mi-primer-repo`.

### 🔸 Opción B: Desde Visual Studio Code

1. Abre VS Code.
2. Haz clic en **Archivo > Abrir carpeta...** y elige `mi-primer-repo`.
3. Si no existe, puedes crearla desde ahí mismo.

---

## 🧠 2. Abre la terminal desde VS Code

1. Una vez estés dentro de tu carpeta, pulsa:
   - `Ctrl + ñ` en Windows o Linux
   - `Control + ~` en Mac
2. Se abrirá la terminal integrada justo abajo.

---

## 🧰 3. Inicia el repositorio con Git

En esa terminal escribe:

```bash
git init
````

> Este comando activa Git en tu proyecto. Ahora Git podrá llevar el control de los archivos.

---

## 🌐 4. Crea tu primer archivo web

Desde el **explorador lateral** de VS Code:

1. Haz clic derecho en tu carpeta y elige **"Nuevo archivo"**.
2. Escribe el nombre: `index.html`
3. Pega este contenido básico:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Mi primera web</title>
  </head>
  <body>
    <h1>¡Hola mundo!</h1>
    <p>Estoy aprendiendo Git 🚀</p>
  </body>
</html>
```

4. Guarda el archivo (`Ctrl + S` o `Cmd + S`).

---

## 🔎 5. Ver el estado del repositorio

En la terminal:

```bash
git status
```

Verás que `index.html` aparece en rojo (Git sabe que existe, pero aún no lo estás controlando).

---

## 📦 6. Añadir archivos a Git

Para decirle a Git que quieres guardar ese archivo:

```bash
git add index.html
```

O si tienes varios archivos:

```bash
git add .
```

---

## 💬 7. Hacer tu primer commit

Ahora vas a guardar ese cambio con una descripción:

```bash
git commit -m "Primer commit: añado index.html con hola mundo"
```

> ✏️ Este mensaje debe explicar lo que hiciste.

---

## 🧭 8. Consultar historial

Para ver los commits que llevas hechos:

```bash
git log
```

Para salir del historial, pulsa `q`.

---

## 🔁 9. Ver diferencias antes de guardar

Si editas el archivo y quieres ver qué cambió:

```bash
git diff
```

---

## ✅ Resumen visual de los comandos

```bash
git init                   # Activar Git en tu carpeta
git status                # Ver el estado actual
git add .                 # Añadir todos los archivos al control de versiones
git commit -m "mensaje"   # Guardar una versión con un mensaje
git log                   # Ver historial de cambios
```

---

👉 Siguiente lección: [03 - Repos remotos en GitHub](https://github.com/Yelose/git-tutorial-webdev/blob/main/03-rutas-y-repos-remotos/README.md)



