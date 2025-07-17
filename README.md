# Problema de "Aliens y Reproducción"


## Descripción del Problema

Tienes una población inicial de aliens, representada como un **array de números**. Cada número indica cuántos días faltan para que ese alien se reproduzca.

Reglas:

- Cuando el contador de un alien llega a **cero**:
  - Se reproduce: crea un nuevo alien con valor inicial 8.
  - Su contador se reinicia a 6.
  - El nuevo alien empieza su ciclo en 8.

El proceso se repite por **X días** y al final debes calcular cuántos aliens hay en total.

---

## Ejemplo Claro - Primera Parte

Población inicial:

```typescript
const initialAliens = [3,4,3,1,2];
const days = 1;
```

Al pasar el primer día, los valores bajan en 1:

```
[2,3,2,0,1]
```

El siguiente día, el cuarto alien (el que estaba en 0) se reproduce:

- Se convierte en 6
- Se agrega un nuevo alien en 8

Resultado después de ese día:

```
[1,2,1,6,0,8]
```

---
## Pregunta 1
Puedes decir cuantos aliens habrá para el día 18
## Pregunta 2
Puedes decir cuantos alien habrá para el día 100
