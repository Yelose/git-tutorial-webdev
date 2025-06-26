# Ejercicios de Repaso: Git y GitHub

En esta sección vas a practicar todo lo aprendido con **dos ejercicios prácticos**:

1. 🧍‍♀️ Ejercicio individual: crea tu primer portafolio personal.
2. 🤝 Ejercicio en grupo: colabora en un proyecto común usando ramas y pull requests.

---

## 🧍‍♀️ Ejercicio individual: Mi portafolio personal

### 🎯 Objetivo

Crear un portafolio web simple donde mostrar quién eres, qué estás aprendiendo y tus primeros proyectos.

### 📋 Pasos

1. Crea una carpeta llamada `mi-portafolio` y ábrela en VS Code.
2. Crea un archivo `index.html` con esta estructura mínima:

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Mi Portafolio</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <h1>Tu nombre aquí</h1>
    <p>Una breve presentación personal.</p>

    <h2>Proyectos</h2>
    <ul>
      <li>Proyecto 1</li>
      <li>Proyecto 2</li>
    </ul>

    <h2>Contacto</h2>
    <p>Email: tu@email.com</p>
  </body>
</html>
```

3. Crea un archivo `style.css` y añade diseño básico (colores, fuente, márgenes...).
4. Inicializa un repositorio con Git, haz commit y súbelo a GitHub.
5. Publica tu portafolio con GitHub Pages.
6. Comparte el enlace con tu profesora o clase.

### ⭐ Extra

* Añade una foto o avatar.
* Usa una fuente externa con Google Fonts.
* Enlaza tu cuenta de GitHub, correo o redes.

---

## 🤝 Ejercicio en grupo: Recetas familiares

### 🎯 Objetivo

Colaborar en un proyecto real compartido, con ramas independientes por funcionalidad (receta), usando pull requests para unir cambios al proyecto principal.

### 👨‍👩‍👧‍👦 Organización

* Forma un grupo de 3 o 4 personas.
* Una persona del grupo crea un repositorio llamado `recetas-familiares`.
* Los demás lo clonan con:

```bash
git clone https://github.com/usuario/recetas-familiares.git
```

### 📋 Tareas

1. **El creador del repo**:

   * Sube un archivo `index.html` con estructura mínima y un comentario como `<!-- Aquí irán las recetas -->`.
   * Activa GitHub Pages.
   * Comparte el repo con el grupo.

2. **Cada alumno**:

   * Escoge una receta (ej: "tarta de queso").

   * Crea una rama con el nombre de la receta (en minúsculas y con guiones):

     ```bash
     git checkout -b tarta-de-queso
     ```

   * Añade la receta dentro de `index.html`:

     ```html
     <section>
       <h2>Tarta de queso</h2>
       <h3>Ingredientes</h3>
       <ul>
         <li>Queso crema</li>
         <li>Huevos</li>
         <li>Azúcar</li>
         ...
       </ul>
       <h3>Pasos</h3>
       <ol>
         <li>Mezcla los ingredientes</li>
         <li>Hornea 40 minutos</li>
         ...
       </ol>
     </section>
     ```

   * Guarda, haz commit y sube la rama:

     ```bash
     git add .
     git commit -m "Añadir receta de tarta de queso"
     git push origin tarta-de-queso
     ```

   * Abre un Pull Request en GitHub hacia la rama `main`.

3. **El creador del repo** revisa y fusiona cada PR.

4. Verifican juntos que el sitio web publicado en GitHub Pages funciona y muestra todas las recetas.

---

## 🧠 Qué estás practicando

✅ Trabajo individual con Git y GitHub
✅ Publicación de proyectos reales en la web
✅ Ramas y flujo profesional de colaboración
✅ Pull Requests y revisión de código
✅ Documentación clara y trabajo en equipo

---

🎓 ¡Con estos ejercicios estás aplicando prácticas reales que usan los desarrolladores en su día a día!

