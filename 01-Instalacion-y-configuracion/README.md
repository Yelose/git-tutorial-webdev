# 01 - Instalación y Configuración de Git

Antes de empezar a usar Git, tenemos que instalarlo en nuestro ordenador y configurarlo por primera vez.

---

## 🧩 1. Instalar Git

### 🔵 Windows
1. Ve a: [https://git-scm.com/download/win](https://git-scm.com/download/win)
2. Descarga el instalador.
3. Ejecuta el archivo `.exe` descargado.
4. Deja las opciones por defecto y pulsa “Siguiente” hasta que se instale si eres principiante.

### 🍎 macOS
1. Abre la terminal y escribe:
   ```bash
   git --version
   ```

2. Si no está instalado, macOS te ofrecerá instalarlo con Xcode Command Line Tools.

O bien puedes descargarlo desde [https://git-scm.com/download/mac](https://git-scm.com/download/mac)

### 🐧 Linux (Debian, Ubuntu...)

```bash
sudo apt update
sudo apt install git
```

---

## ⚙️ 2. Configurar Git por primera vez

Una vez instalado, debes indicarle a Git quién eres. Abre la terminal y escribe:

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tucorreo@example.com"
```

Puedes comprobar que se ha guardado correctamente con:

```bash
git config --list
```

---

## 📂 3. Crear una carpeta de práctica

1. Crea una carpeta donde guardarás tus proyectos de prueba:

   * Por ejemplo: `git-ejercicios`

2. Entra en esa carpeta desde la terminal:

   ```bash
   cd ruta/a/git-ejercicios
   ```

3. ¡Ya puedes iniciar tu primer repositorio en la siguiente lección!

---

## 🧠 Recuerda

* Estos datos (`user.name` y `user.email`) aparecerán en cada commit que hagas.
* Sólo necesitas configurarlos una vez si usas `--global`.
* Puedes cambiarlos cuando quieras con los mismos comandos.

---

👉 Ve ahora a la [lección 02 - Comandos básicos](../02-comandos-basicos) para comenzar a usar Git.


---
