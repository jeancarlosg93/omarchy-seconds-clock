# Omarchy Seconds Clock

Reloj de Omarchy Quattro que actualiza y muestra los segundos, conservando el calendario y los controles del reloj original. Al instalarlo sustituye la entrada `omarchy.clock` existente, sin añadir un segundo reloj. Incluso si tu configuración guardaba un formato sin segundos, el plugin los añade a la visualización.

## Instalar

```bash
omarchy plugin add https://github.com/jeancarlosg93/omarchy-seconds-clock.git --enable
omarchy restart shell
```

No requiere la barra de píldoras ni el plugin de espacios de trabajo.

Abre el calendario con clic izquierdo y pulsa el engranaje **CLOCK APPEARANCE** para ajustar el formato, la familia tipográfica y el tamaño de la letra (8–20 px, para caber en la barra). Los cambios se guardan en la entrada del reloj de `~/.config/omarchy/shell.json`. El formato utiliza los códigos de Qt, por ejemplo `ddd d MMM HH:mm:ss`; si eliges un formato personalizado, puedes incluir u omitir `ss`. Deja la fuente o el tamaño en blanco para seguir el valor del tema/sistema. El clic derecho sobre el reloj sigue recorriendo formatos predefinidos.

Para volver al reloj original: `omarchy plugin disable jeanc.clock`. Para actualizar: `omarchy plugin update jeanc.clock`.

El código deriva del reloj de [Omarchy](https://github.com/omacom/omarchy), bajo licencia MIT. Véase [LICENSE](LICENSE).
