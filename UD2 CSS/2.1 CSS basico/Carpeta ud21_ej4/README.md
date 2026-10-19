# Respuestas al Ejercicio 4

## Parte A - Selector de id

### 1. Mensaje de error del validador W3C
*(Nota: Para obtener tu error exacto, debiste poner `<h2 id="corp">` temporalmente en tu HTML y pasarlo por https://validator.w3.org/)*

Al duplicar a propósito el `id="corp"` en el elemento `<h2>`, el validador del W3C arrojó un error similar a este:

> **Error**: Duplicate ID `corp`.
> **Warning**: The first occurrence of ID `corp` was here.

### 2. ¿Por qué se desaconseja usar selectores de id para estilizar en CSS?
Aunque técnicamente funciona, se desaconseja usar selectores de ID (`#mi-id`) en CSS por dos motivos principales:

1.  **Falta de reutilización:** Por definición en HTML, un ID debe ser único en toda la página. Si estilizas un botón usando su ID, no podrás aplicar ese mismo estilo visual a otro botón en la misma página. Las clases (`.mi-clase`), en cambio, están diseñadas para ser reutilizadas múltiples veces.
2.  **Problemas de especificidad:** Los selectores de ID tienen un peso (especificidad) extremadamente alto en CSS. Si intentas sobreescribir el estilo de un elemento que tiene un ID utilizando una clase más adelante en tu hoja de estilos, el CSS no te hará caso porque el ID "gana". Esto hace que el código sea muy difícil de mantener y modificar a largo plazo.