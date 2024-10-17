# Git Cheat Sheet

## Configuración Inicial
```bash
# Configura tu nombre de usuario
git config --global user.name "Tu Nombre"

# Configura tu dirección de correo electrónico
git config --global user.email "tuemail@example.com"

# Ver configuración actual
git config --list
```

## Creación de Repositorios
```bash
# Crear un nuevo repositorio
git init nombre-del-repositorio

# Clonar un repositorio existente
git clone url-del-repositorio
```

## Comandos Básicos
```bash
# Ver el estado del repositorio
git status

# Ver cambios no confirmados
git diff

# Añadir cambios al área de preparación
git add nombre-del-archivo
git add . # Añadir todos los cambios

# Confirmar cambios
git commit -m "Mensaje de confirmación"
```

## Ramas
```bash
# Listar ramas
git branch

# Crear una nueva rama
git branch nombre-de-la-rama

# Cambiar a otra rama
git checkout nombre-de-la-rama

# Crear y cambiar a una nueva rama
git checkout -b nombre-de-la-rama
```

## Traer Cambios de una Rama
```bash
# Obtener los últimos cambios del repositorio remoto
git fetch origin

# Traer cambios de una rama remota
git checkout nombre-de-la-rama
git pull origin nombre-de-la-rama
```

## Merging (Fusión)
```bash
# Cambiar a la rama principal (por ejemplo, main)
git checkout main

# Fusionar otra rama en la rama actual
git merge nombre-de-la-rama
```

## Resolución de Conflictos
```bash
# Después de un merge, si hay conflictos
# Abre los archivos en conflicto y resuélvelos

# Añadir los archivos resueltos al área de preparación
git add nombre-del-archivo

# Confirmar la fusión
git commit -m "Resuelto conflicto de fusión"
```

## Sincronización con el Repositorio Remoto
```bash
# Enviar cambios locales al repositorio remoto
git push origin nombre-de-la-rama

# Obtener y fusionar cambios del repositorio remoto
git pull origin nombre-de-la-rama
```

## Otras Comandos Útiles
```bash
# Ver el historial de confirmaciones
git log

# Ver el historial en formato gráfico
git log --graph --oneline --all

# Deshacer cambios en un archivo específico
git checkout -- nombre-del-archivo

# Deshacer la última confirmación (sin perder los cambios)
git reset HEAD~1

# Deshacer la última confirmación y eliminar cambios
git reset --hard HEAD~1
```

## Trabajando con Tags
```bash
# Crear una nueva etiqueta
git tag -a v1.0 -m "Versión 1.0"

# Ver etiquetas
git tag

# Enviar etiquetas al repositorio remoto
git push origin --tags
```

## Eliminar Ramas
```bash
# Eliminar una rama local
git branch -d nombre-de-la-rama

# Eliminar una rama remota
git push origin --delete nombre-de-la-rama
```

## Nota
Recuerda que antes de realizar fusiones y eliminaciones, siempre es recomendable hacer una copia de seguridad de tu trabajo.
```

Guarda este contenido en un archivo con extensión `.md`, y tendrás una cheat sheet fácil de usar para tus operaciones con Git. Si necesitas añadir más detalles o comandos específicos, ¡hazmelo saber!
