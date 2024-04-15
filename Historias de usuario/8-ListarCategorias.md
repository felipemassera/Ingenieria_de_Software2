## Título:
Listar Categorías
## Narrativa:
- Como Administrador
- Quiero visualizar el listado de categorías
- Para gestionar las categorías que se encuentran en el sistema
## Reglas de Negocio
- N/A
## Criterios de aceptación:
- **Escenario 1: Listar categorías exitoso**
    + **Dado** que se pudo recuperar los información de categorías existentes en el sistema.
    + **Cuando** se ingrese a la interfaz de manejo de categorías. 
    + **Entonces** el sistema muestra en pantalla un listado de las categorías cargadas en el sistema junto con las opciones para modificar **Y** eliminar las mismas.

- **Escenario 2: Listado Vacío**
    + **Dado** que no se pudo recuperar la información de que exista alguna categoría en el sistema.
    + **Cuando** se ingrese a la interfaz de manejo de categorías.
    + **Entonces** el sistema muestra en pantalla el mensaje "No se ha podido encontrar categorías en el sistema".