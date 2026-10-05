# claude-plugins

Marketplace `gontzalo`: plugins y mods para Claude Code (terminal y Code tab del desktop).

## Plugins

| Plugin | Qué hace |
|---|---|
| [usage-pace](https://github.com/diazgonza17/usage-pace) | Muestra arriba del input el % usado de la sesión de 5 horas, lo esperado a esta altura y el tiempo al reset, con Isaac reaccionando a tu ritmo |

## Instalación

Agregá el marketplace una vez:

```
/plugin marketplace add diazgonza17/claude-plugins
```

Y después instalá cada plugin por su nombre:

```
/plugin install usage-pace@gontzalo
```

Desde la terminal es lo mismo con `claude plugin marketplace add` y `claude plugin install`. Cada plugin explica en su README cómo se configura.

## Actualizar

```
/plugin marketplace update gontzalo
```

## Cómo está armado

Este repo es solo el catálogo: [`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json) lista cada plugin y apunta al repo donde vive su código. Cada plugin publica sus versiones en su propio repo, subiendo `version` en su `plugin.json`; el catálogo se toca solo para sumar un plugin o cambiar su descripción.
