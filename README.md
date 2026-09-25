# Omarchy Seconds Clock

Reloj de Omarchy Quattro que actualiza y muestra los segundos, conservando el calendario y los controles del reloj original. Al instalarlo sustituye la entrada `omarchy.clock` existente, sin añadir un segundo reloj. Incluso si tu configuración guardaba un formato sin segundos, el plugin los añade a la visualización.

## Instalar

```bash
omarchy plugin add https://github.com/jeancarlosg93/omarchy-seconds-clock.git --enable
omarchy restart shell
```

No requiere la barra de píldoras ni el plugin de espacios de trabajo.

Abre el calendario con clic izquierdo y pulsa el engranaje **CLOCK APPEARANCE** para elegir un formato rápido o editarlo libremente, buscar entre las fuentes instaladas, seleccionar un tamaño (8–20 px) y activar negrita o cursiva. La vista previa muestra el resultado antes de pulsar **Save changes**. Los cambios se guardan en la entrada del reloj de `~/.config/omarchy/shell.json` y sobreviven al reinicio del shell. El formato utiliza los códigos de Qt, por ejemplo `ddd d MMM HH:mm:ss`; si eliges uno personalizado, puedes incluir u omitir `ss`. Las opciones *System font* y *System size* siguen el tema del sistema. El clic derecho sobre el reloj sigue recorriendo formatos predefinidos.

También puedes abrir directamente el panel de ajustes con `quickshell ipc -p /usr/share/omarchy/shell/shell.qml call omarchy.clock customize`.

Para volver al reloj original: `omarchy plugin disable jeanc.clock`. Para actualizar: `omarchy plugin update jeanc.clock`.

El código deriva del reloj de [Omarchy](https://github.com/omacom/omarchy), bajo licencia MIT. Véase [LICENSE](LICENSE).
