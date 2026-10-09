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
git add .
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

| Tipo | Significado | Cuándo utilizarlo |
|---|---|---|
| `build` | Compilación | Cambias dependencias o configuración de compilación |
| `ci` | Integración continua | Modificas automatizaciones de pruebas o despliegues |
| `docs` | Documentación | Modificas un README.md |
| `feat` | Nueva funcionalidad | Añades una función al programa |
| `fix` | Corrección | Arreglas un error |
| `perf` | Rendimiento | Haces que el programa funcione más rápido |
| `refactor` | Reestructuración | Mejoras el código sin cambiar su comportamiento |
| `style` | Estilo | Corriges espacios, indentación o formato |
| `test` | Pruebas | Añades o corriges pruebas |

Ejemplos:


| Lo que haces | Commit |
|---|---|
| Creas un programa | `feat: añadir programa inicial` |
| Corriges un `if` | `fix: corregir condición` |
| Modificas el README | `docs: actualizar instrucciones` |
| Ordenas el código | `refactor: simplificar función` |
| Corriges indentación | `style: corregir indentación` |
| Añades pruebas | `test: añadir pruebas de cálculo` |
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