# Simulador de Patchbay · Estudio A

Simulador educativo del patchbay del Estudio A (consola Neve Genesys) para que los alumnos practiquen el ruteo de señal sin depender del estudio físico.

## Qué hace

- Reproduce las 6 secciones del patchbay (576 jacks) con los nombres reales de cada punto, tomados del levantamiento fotográfico del patchbay (Rev. 04).
- No simula audio real: es un simulador de **flujo de señal** — conecta cables virtuales entre jacks SUP e INF y valida rutas.
- **Modo Sandbox**: patcheo libre, se guarda en el navegador de cada alumno.
- **Modo Ejercicios**: consignas de ruteo reales (insertar un compresor en un canal, mandar una señal a un outboard y traer el retorno, exportar un stem al DAW, etc.) con verificación automática.

## Estado de los datos

Las zonas marcadas con textura rayada en la interfaz corresponden a posiciones que las fotos originales del patchbay no permiten confirmar con certeza (etiqueta deslavada, sin conector visible, o fuera de alcance). Estas zonas se dejan así intencionalmente por ahora; se pueden corregir editando el arreglo `SECTIONS` en `index.html` a medida que se verifiquen en el estudio.

## Uso

Es una página estática de un solo archivo (`index.html`), sin dependencias de build. Para verla:

- Ábrela localmente en un navegador, o
- Publícala con GitHub Pages (Settings → Pages → Deploy from branch → `main` / raíz).

## Próximos pasos posibles

- Confirmar en el estudio las zonas marcadas "sin confirmar" y actualizar los datos.
- Sumar una franja de canal simplificada (gain, HPF, pan, assign) para conectar el patcheo con lo que el alumno ajusta en consola.
- Ampliar la lista de ejercicios.
