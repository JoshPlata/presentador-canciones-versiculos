# Contexto del proyecto: Cantos · Presentación

## Propósito
Página HTML independiente para presentar letras de canciones en diapositivas. Se abre directamente en un navegador y no requiere servidor.

## Archivos
- `Presentador.html`: aplicación completa, estilos, animaciones y lógica de presentación.
- `mis-canciones.json`: biblioteca inicial de canciones. El HTML puede cargarla desde **Cargar archivo** y descargar una versión actualizada desde **Guardar canciones**.

## Funciones actuales
- Índice de canciones ordenado alfabéticamente; permite añadir, editar y eliminar canciones.
- La letra se divide en diapositivas usando líneas en blanco como separadores.
- Controles de anterior/siguiente, teclado y pantalla completa.
- El índice se puede ocultar y mostrar.
- Fondos seleccionables: Aurora, Partículas, Ondas, Estrellas y Estático. La selección se recuerda en `localStorage`.
- Las canciones también se guardan en `localStorage` del navegador. Para mover la biblioteca entre equipos, cargar y guardar el JSON desde la interfaz.

## Notas de mantenimiento
- Mantén el HTML autocontenido; no necesita herramientas de compilación.
- El contenido inicial de «Gracia sublime» está en el HTML y en el JSON. Si se cambia, mantén ambos sincronizados.
- Al importar una biblioteca, el archivo JSON debe contener una propiedad `songs` con elementos que incluyan `title` y `lyrics`; `artist` es opcional.
- Las animaciones están hechas con CSS. Conserva la legibilidad de las letras y el soporte de movimiento reducido.
- Evita modificar o reemplazar el JSON de la persona usuaria sin conservar primero sus canciones.

## Presentador de versículos
- `Presentador.html` tiene dos modos independientes: canciones y versículos.
- Las citas usan `localStorage` key `cantos-verses`; exportan/importan `mis-versiculos.json` con `{format: "presentador-verses-v1", verses: [{id, reference, version, text}]}`.
- Mantén separada la biblioteca de versículos de `cantos-songs` y `mis-canciones.json`.
