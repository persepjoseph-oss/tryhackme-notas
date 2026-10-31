# OverTheWire Bandit - Niveles 0 a 6

**Fecha:** 31 de octubre de 2026
**Enlace:** https://overthewire.org/wargames/bandit/

> No publico las contraseñas de los niveles: son las respuestas del juego.
> Aquí solo anoto los comandos y lo que aprendí.

## Cómo me conecto
```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
La contraseña de cada nivel se obtiene resolviendo el nivel anterior.

## Lo que practiqué

| Nivel | Reto | Comando que usé | Qué aprendí |
|---|---|---|---|
| 0 | Conectarme por SSH | `ssh bandit0@... -p 2220` | Entrar a un servidor Linux remoto |
| 1 | Archivo llamado `-` | `cat ./-` | `cat -` se queda esperando porque `-` significa "leer lo que escribo". Con `./` indico que es un archivo de esta carpeta |
| 2 | Nombre con espacios | `cat "./--spaces in this filename--"` | Los nombres con espacios van entre comillas |
| 3 | Archivo oculto | `find inhere` (o `ls -a`) | `ls` no muestra los archivos que empiezan con punto |
| 4 | (completar con lo que hice) | | |
| 5 | Archivo por tamaño | `find . -size 1033c` | `find` también busca por tamaño; la `c` son bytes |
| 6 | Dueño, grupo y tamaño | `find / -user bandit7 -group bandit6 -size 33c 2>/dev/null` | `find` puede filtrar por dueño y grupo; `2>/dev/null` esconde los errores de permiso denegado |

## Errores que cometí
- `cat -` se quedó esperando: lo cancelé con Ctrl+C.
- `find "dashed filename"` no existe: `find` busca por ruta, no por la descripción del enunciado.
- `cat inhere` dio error: `cat` lee archivos, no carpetas.

## Qué me costó
- Entender por qué `ls` no mostraba todos los archivos.
- Recordar la sintaxis de `find` sin mirar.

## Siguiente paso
Niveles 7 a 10: `grep`, `sort` con `uniq`, `strings` y `base64`.
