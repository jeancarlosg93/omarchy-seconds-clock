# Omarchy Seconds Clock

Reloj de Omarchy Quattro que actualiza y muestra los segundos, conservando el calendario y los controles del reloj original. Al instalarlo sustituye la entrada `omarchy.clock` existente, sin añadir un segundo reloj. Incluso si tu configuración guardaba un formato sin segundos, el plugin los añade a la visualización.

## Instalar

```bash
omarchy plugin add https://github.com/jeancarlosg93/omarchy-seconds-clock.git --enable
omarchy restart shell
```

No requiere la barra de píldoras ni el plugin de espacios de trabajo.

Para volver al reloj original: `omarchy plugin disable jeanc.clock`. Para actualizar: `omarchy plugin update jeanc.clock`.

El código deriva del reloj de [Omarchy](https://github.com/omacom/omarchy), bajo licencia MIT. Véase [LICENSE](LICENSE).
