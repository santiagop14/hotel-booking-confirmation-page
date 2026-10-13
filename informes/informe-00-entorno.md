# Informe 00 — Entorno (Proyecto 01: Hotel booking confirmation page)

> Leyenda de fuentes:
> - **[Verificado]** = comprobado con comandos de solo lectura (`git status`, `git log --oneline`, `git remote -v`, `git show --stat`, `ls`) el 2026-10-13.
> - **[Según el usuario]** = dato aportado por el usuario que no se pudo verificar.

## 1. Objetivo de la etapa

Dejar listo el entorno de trabajo del Proyecto 01 (desafío "Hotel booking confirmation page" de Frontend Mentor, HTML y CSS): un repositorio Git propio, conectado a GitHub, con los archivos iniciales del desafío y el `CLAUDE.md` para que Claude Code lo lea.

## 2. Qué se hizo (paso a paso)

1. **[Según el usuario]** Se creó el repositorio en la página de GitHub (público, llamado `hotel-booking-confirmation-page`) y se trajo al equipo con `git clone`.
2. **[Según el usuario]** Primer intento fallido: el clone quedó anidado dentro de la carpeta del starter. Al intentar mover la carpeta, Windows mostró "el archivo está siendo utilizado en otro proceso". Solución: clonar de nuevo en una carpeta limpia.
3. **[Según el usuario]** Se copiaron los archivos del starter al clone. La primera copia con `Get-ChildItem -Exclude` no copió nada y no mostró error; se corrigió usando `Where-Object`.
4. **[Según el usuario]** `CLAUDE.md` venía como `# CLAUDE.md — Portafolio de Desarro.txt`; se renombró a `CLAUDE.md`.
5. **[Verificado]** Se hizo un primer commit: `2ea73dd chore: add Frontend Mentor starter files and project CLAUDE.md` (sobre el `505e6fe Initial commit` previo).
6. **[Según el usuario]** El commit se subió con `git push -u origin main`.

## 3. Archivos creados o modificados

Según `git show --stat HEAD` **[Verificado]**, el commit `2ea73dd` cambió 37 archivos (2310 inserciones, 2 eliminaciones):

| Archivo / carpeta | Por qué |
|---|---|
| `CLAUDE.md` | Documento maestro de reglas y metodología para Claude Code. |
| `AGENTS.md` | Instrucciones para agentes de IA, parte del starter de Frontend Mentor. |
| `README.md` (modificado) | Venía en el starter; el commit lo modificó (la fecha de modificación exacta del contenido no se revisó). |
| `README-template.md` | Plantilla de README del starter. |
| `style-guide.md` | Guía de estilo del desafío (colores, tipografías). |
| `index.html` | HTML inicial del starter (125 líneas añadidas). No se tocó en esta tarea. |
| `.gitignore` | Evita subir dependencias, `.env`, archivos de editor, etc. |
| `assets/fonts/` | Fuentes DM Mono, DM Sans y Fraunces con sus licencias (OFL.txt). |
| `assets/images/` | Íconos SVG, logo, ilustración y favicon del desafío. |
| `design/` | Imágenes de referencia: escritorio, móvil, menú móvil y estados activos. |
| `preview.jpg` | Imagen de vista previa del desafío. |

Archivo creado en esta tarea: `informes/informe-00-entorno.md` (este informe), aún sin commit.

## 4. Conceptos aprendidos

**[Según el usuario]** (lo siguiente es lo que el usuario reportó como lecciones; no se verificó):
- Un comando sin salida puede no haber hecho nada: se verifica con `git status`.
- Los avisos "LF will be replaced by CRLF" reflejan una diferencia de saltos de línea en Windows; no son un error.

**[Verificado]** Conceptos que aparecen en el repositorio: repositorio local vs. remoto (`origin`), commit, rama `main` y seguimiento de rama remota, y el formato Conventional Commits (el commit usa el prefijo `chore:`).

## 5. Problemas o advertencias encontradas

Todos **[Según el usuario]**:
- Clone anidado en la carpeta del starter; el movimiento falló por archivo en uso en Windows. Resuelto clonando de nuevo en una carpeta limpia.
- Copia con `Get-ChildItem -Exclude` que no copió nada y no dio error. Resuelto con `Where-Object`.
- `CLAUDE.md` con nombre incorrecto (`.txt`). Renombrado.
- Avisos LF/CRLF: no son un error.
- Existe una carpeta de respaldo `PROYECTO HOTEL` fuera de este repositorio; no se toca.

## 6. Cómo se comprobó que todo funciona

**[Verificado]**:
- `git status`: `On branch main`, `Your branch is up to date with 'origin/main'`, `nothing to commit, working tree clean`.
- `git log --oneline`: dos commits, `2ea73dd` y `505e6fe`.
- `git remote -v`: `origin` apunta a `https://github.com/santiagop14/hotel-booking-confirmation-page.git` (fetch y push).
- Listado de la raíz: `.gitignore`, `AGENTS.md`, `CLAUDE.md`, `README.md`, `README-template.md`, `style-guide.md`, `index.html`, `preview.jpg`, `assets/` y `design/`.

Nota: "up to date with 'origin/main'" compara con la última referencia remota conocida localmente; no se hizo `git fetch` para confirmarlo contra GitHub. Que el repositorio sea público en GitHub es dato **[Según el usuario]**.

## 7. Siguiente paso

Etapa 1 (según la metodología de `CLAUDE.md`): análisis del desafío, es decir, revisar requisitos, `style-guide.md`, `README.md` y las imágenes de `design/`, identificar qué conocimientos de HTML y CSS se necesitan y armar un plan antes de escribir código. Antes, guardar este informe con Git (ver comandos entregados en la conversación).
