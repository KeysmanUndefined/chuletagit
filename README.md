# Git - Comandos básicos

## 1. Crear un repositorio desde una carpeta existente

Entrar en la carpeta del proyecto:

```bash
cd ruta/del/proyecto
```

Inicializar Git:

```bash
git init
```

Ver el estado:

```bash
git status
```

Añadir los archivos:

```bash
git commit add .
```

Crear el primer commit:

```bash
git commit -m "feat: añadir proyecto inicial"
```

Conectar el repositorio local con GitHub:

```bash
git remote add origin URL_DEL_REPOSITORIO
```

Establecer main como rama principal:

```bash
git branch -M main
```

Subirlo por primera vez:

```bash
git push -u origin main
```

# Trabajo habitual después.

Antes de empezar:

```bash
git pull
```

Después de modificar archivos:

```bash
git status
git add .
git commit -m "feat: descripción del cambio"
git push
```

Descargar un repositorio que ya existe:

```bash
git clone URL_DEL_REPOSITORIO
```

Entrar en él:

```bash
cd nombre-repositorio
```

Abrirlo en VS Code:

```bash
code .
```

## **Después ya no se vuelve a hacer clone.**
Para traer cambios:

```bash
git pull
```

## Comandos para saber dónde estoy
Ver la carpeta actual:

```bash
pwd
```

Ver los archivos:

```bash
ls
```

Ver los commits:

```bash
git log --oneline
```

Ver a qué repositorio de GitHub está conectado:

```bash
git remote -v
```
## Conventional Commits
Ejemplos:

```bash
git commit -m "feat: añadir comprobación de números primos"
git commit -m "fix: corregir cálculo de divisores"
git commit -m "docs: actualizar README"
git commit -m "refactor: simplificar función is_prime"
git commit -m "test: añadir pruebas para números negativos"
```

## Regla rápida
Repositorio que NO tengo en el ordenador:

```bash
git clone
```

Repositorio que YA tengo:

```bash
git pull
```

Después de trabajar:

```bash
git add .
git commit -m "tipo: descripción"
git push
```