# 04 - Ramas y Colaboración

Git permite trabajar en varias versiones del mismo proyecto al mismo tiempo. Esto se hace mediante **ramas** (branches), y es clave cuando quieres **experimentar sin romper el proyecto principal** o colaborar con otras personas.

---

## 🌱 ¿Qué es una rama?

Imagina que tu proyecto es un árbol. La rama principal se llama `main`. Si creas una rama nueva, es como sacar una ramita lateral para probar algo sin afectar al tronco.

Cuando terminas tu trabajo en esa rama, puedes **fusionarla** (`merge`) con la rama principal.

---

## 🛠️ 1. Crear una nueva rama

```bash
git branch nombre-de-la-rama
```

Ejemplo:

```bash
git branch mi-experimento
```

---

## 🔁 2. Cambiar de rama

```bash
git checkout nombre-de-la-rama
```

O bien, desde Git 2.23 puedes usar:

```bash
git switch nombre-de-la-rama
```

> Git cambiará los archivos de tu carpeta al estado de esa rama. ¡No olvides guardar tus cambios antes de cambiar de rama!

---

## 🌳 3. Crear y cambiar de rama al mismo tiempo

```bash
git checkout -b nombre-nuevo
```

Ejemplo:

```bash
git checkout -b nuevo-boton
```

---

## 🔀 4. Fusionar ramas (merge)

1. Vuelve a la rama principal:

```bash
git switch main
```

2. Fusiona los cambios de la otra rama:

```bash
git merge nombre-de-la-rama
```

Ejemplo:

```bash
git merge nuevo-boton
```

---

## 🧹 5. Borrar una rama (opcional)

Después de hacer merge, puedes borrar la rama:

```bash
git branch -d nombre-de-la-rama
```

---

## 🤝 6. Clonar un repositorio de otra persona

Si un compañero tiene su proyecto en GitHub, puedes copiarlo con:

```bash
git clone https://github.com/usuario/nombre-repo.git
```

Eso crea una copia en tu ordenador, con historial incluido.

---

## 🧭 Comandos usados en esta lección

```bash
git branch nombre        # Crea una nueva rama
git switch nombre        # Cambia de rama
git checkout -b nombre   # Crea y cambia de rama a la vez
git merge nombre         # Fusiona una rama con la actual
git branch -d nombre     # Borra una rama
git clone URL            # Clona un repositorio de GitHub
```

---

## 🧠 ¿Cuándo usar ramas?

* Para probar algo sin romper lo que funciona.
* Para desarrollar una nueva funcionalidad sin afectar al resto.
* Para que varias personas trabajen a la vez sin pisarse.

---

👉 Siguiente lección: [05 - Publicar tu web con GitHub Pages](https://github.com/Yelose/git-tutorial-webdev/blob/main/05-publicar-proyecto-html/README.md)

