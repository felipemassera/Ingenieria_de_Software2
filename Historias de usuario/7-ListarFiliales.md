## Título:
Listar Filiales
## Narrativa:
- Como Administrador
- Quiero visualizar el listado de filiales
- Para gestionar las filiales que se encuentran en el sistema
## Reglas de Negocio
- N/A
## Criterios de aceptación:
- **Escenario 1: Listar filiales exitoso**
    + **Dado** que se pudo recuperar los información de filiales existentes en el sistema.
    + **Cuando** se ingrese a la interfaz de manejo de filiales. 
    + **Entonces** el sistema muestra en pantalla un listado de las filiales cargadas en el sistema junto con las opciones para modificar **Y** eliminar las mismas.

- **Escenario 2: Listado Vacío**
    + **Dado** que no se pudo recuperar la información de que exista alguna filial en el sistema.
    + **Cuando** se ingrese a la interfaz de manejo de filiales.
    + **Entonces** el sistema muestra en pantalla el mensaje "No se ha podido encontrar filiales en el sistema".