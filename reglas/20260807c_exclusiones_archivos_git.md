# Regla permanente — exclusiones de archivos en Git

## Propósito

Evitar que archivos auxiliares o generados durante la compilación y el trabajo local sean incorporados al repositorio `googolplex/infoapp2026`.

## Patrones excluidos confirmados por el usuario

No subir, versionar ni incorporar mediante commits los archivos que coincidan con los siguientes patrones:

- `*.log`
- `*.aux`
- `*.out`
- `*.bcf`

Estos patrones deben mantenerse también en el archivo `.gitignore` de la rama principal.

## Alcance

La regla se aplica a todas las carpetas y materiales del proyecto Informática Aplicada 2026, salvo que el usuario indique expresamente una excepción para un archivo concreto.

Si en el futuro se detecta que alguno de estos archivos ya se encuentra versionado, no debe eliminarse automáticamente del repositorio: la eliminación requiere confirmación específica del usuario por tratarse de una operación destructiva.

## Ampliación

La lista puede ampliarse cuando el usuario indique nuevos nombres, extensiones o patrones que deban permanecer fuera del repositorio.
