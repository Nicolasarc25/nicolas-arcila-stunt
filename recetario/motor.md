# Motor — qué hace el sistema cuando mando una foto

Lee siempre antes: `REGLAS.md`, `perfil.md`, `bitacora.md`.

## Paso 1 — Leer la foto y NO pasar de ahí

Devuelve solo el inventario, sin recetas todavía:

```
VEO (seguro):     tomate, huevos (4 visibles), cebolla
VEO (dudoso):     algo verde al fondo — ¿pimiento o calabacín?
NO PUEDO SABER:   cuánto arroz queda en ese paquete
BOTES SIN LEER:   1, en la puerta
```

Y una sola pregunta de cierre: *"¿Corrijo algo antes de seguir?"*

Sin este paso el sistema se inventa la mitad del inventario. Es el paso que
la gente quiere saltarse y el que hace que funcione.

## Paso 2 — Proponer (máximo 3, mínimo 0)

Cada opción, con este esquema exacto:

```
### 1. [Nombre]  ·  ~25 min  ·  2 raciones

CON LO QUE TIENES
  · 3 huevos            DICHO
  · 1 cebolla           VISTO (alta)
  · aceite de oliva     FONDO

TE FALTA — IMPRESCINDIBLE  (sin esto no es este plato)
  · nada

TE FALTA — OPCIONAL  (mejora, no bloquea)
  · perejil        → sin él pierde frescor, no pasa nada
  · nata           → sustituible por un chorro de leche

CANTIDAD SIN CONFIRMAR
  · el arroz: necesito ~180 g. ¿Tienes al menos eso?

PASOS
  1. ...  (rango de tiempo + señal sensorial, nunca número seco)
```

Regla dura: si algo está en IMPRESCINDIBLE, la receta **no** se presenta como
"puedes hacerla". Se presenta como "te falta X para esta".

## Paso 3 — Cerrar el círculo

Después de cocinar, una línea a `bitacora.md`. Es el único mecanismo por el
que esto mejora. Si este paso no se hace, el sistema no aprende nada y es
un chat normal con pasos de más.
