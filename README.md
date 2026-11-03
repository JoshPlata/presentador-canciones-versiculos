# Presentador

Presentación local de letras en diapositivas, hecha en un solo archivo HTML.

## Para empezar

1. Abre `Presentador.html` en Safari, Chrome u otro navegador moderno.
2. Pulsa **Cargar archivo** y selecciona `mis-canciones.json` para cargar la biblioteca incluida.
3. Busca canciones por título o artista en el campo de búsqueda del índice. Selecciona una canción y usa **Siguiente** o la flecha derecha para avanzar.
4. Usa **Pantalla completa** para presentar. Puedes ocultar el índice con el botón **Ocultar índice**.

## Agregar y editar canciones

- Pulsa **+** junto al índice para agregar una canción.
- Usa **Editar canción** para cambiar el título, artista o letra.
- Separa las estrofas con una línea en blanco: cada bloque se mostrará en una diapositiva.
- Las canciones se guardan en el navegador que estés usando.

## Guardar y trasladar la biblioteca

Después de agregar o editar canciones, pulsa **Guardar canciones** para descargar `mis-canciones.json` actualizado. Conserva ese JSON junto al HTML. En otra computadora, abre el HTML y pulsa **Cargar archivo** para seleccionar el JSON actualizado.

El navegador no modifica el archivo JSON automáticamente; hay que pulsar **Guardar canciones** para descargar la versión nueva.

## Fondos y controles

Puedes seleccionar Aurora, Partículas, Ondas, Estrellas o Estático desde el selector de fondo. La preferencia se recuerda en el navegador actual.

- `←` y `→`: diapositiva anterior o siguiente.
- `Espacio`: siguiente diapositiva.
- **Pantalla completa**: entrar o salir del modo de presentación.
- **Ocultar índice / Mostrar índice**: esconder o recuperar la lista de canciones.

## Archivos

- `Presentador.html`: la aplicación y la presentación.
- `mis-canciones.json`: biblioteca de canciones, separada de los versículos.
- `mis-versiculos.json`: biblioteca independiente de versículos.
- `AGENTS.md`: notas de contexto para mantener o ampliar el proyecto.

## Presentar versículos

Pulsa **Versículos** en el panel lateral. Usa **+** para agregar una referencia, versión y texto; busca por referencia o texto en el índice, selecciona una cita y navega con **Anterior/Siguiente** o las flechas del teclado.

La lista de versículos es independiente de las canciones. **Cargar versículos** importa `mis-versiculos.json`; **Guardar versículos** descarga su versión actualizada. El formato es `{ "format": "presentador-verses-v1", "verses": [{ "reference": "Salmo 23:1", "version": "RVR1909", "text": "..." }] }`. Las citas también se guardan en el navegador actual.
