# Evidencias del módulo de Big Data

Oscar Cárdenas Valdez, A01741965.
TC3009C, Inteligencia artificial avanzada para la ciencia de datos, Gpo 602.

Este repositorio es lo que se entregó en Canvas como evidencia de las dos tareas del módulo de Big
Data. Las dos apuntan a este mismo link.

## Evidencia 1. Evaluación de conceptos de homologación

Entrega: 24 de septiembre de 2026, 23:59.

Pide documentar los resultados de la homologación de conceptos hecha en clase, con la captura de los
resultados de las 7 pruebas y cuestionarios del notebook de NotebookLM
`070ad3e4-e3c0-4320-b59d-7b73564d981c`.

Pendiente. El notebook no abre con la cuenta del Tec ni con las otras cuentas del perfil, responde
"You need access", y la cuenta no tiene notebooks propios. Las capturas van en
`evidencia-1-homologacion/capturas/` en cuanto se resuelva el acceso.

## Evidencia 2. Análisis del caso de éxito de Uber

Entrega: 24 de septiembre de 2026, 23:59. Ventana abierta hasta el 25 de septiembre, 23:59.

Respuestas a las cinco preguntas de discusión del caso: las tres preguntas detonantes de la sección 5
y las dos del debrief. Incluye una conexión con el Reto A de Ternium y una nota sobre dos cifras del
documento fuente que no cuadran entre sí.

- [`evidencia-2-uber/Evidencia2_Uber_A01741965.pdf`](evidencia-2-uber/Evidencia2_Uber_A01741965.pdf), el entregable.
- [`evidencia-2-uber/evidencia2_uber.html`](evidencia-2-uber/evidencia2_uber.html), la fuente con la que se genera el PDF.

El PDF se regenera con Chromium vía playwright:

```bash
python -c "from playwright.sync_api import sync_playwright as s; from pathlib import Path; p=s().start(); b=p.chromium.launch(); pg=b.new_page(); pg.goto(Path('evidencia-2-uber/evidencia2_uber.html').resolve().as_uri()); pg.emulate_media(media='print'); pg.pdf(path='evidencia-2-uber/Evidencia2_Uber_A01741965.pdf', format='A4'); b.close(); p.stop()"
```

## Fuente del caso

Peña González, J. A. (2026). *Big data - Clase 1 - Caso Estudio Uber*. TC3009C, Tecnológico de
Monterrey. Documento de clase, compartido en solo lectura.
