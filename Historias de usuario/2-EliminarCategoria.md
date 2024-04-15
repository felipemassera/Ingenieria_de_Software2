## Título:
Eliminar categoría

## Narrativa:
- Como Administrador/Ayudante
- Quiero eliminar una categoría
- Para organizar el listado de productos

## Reglas de Negocio

## Criterios de aceptación:
- **Escenario 1: Eliminar Categoría exitoso**
    + **Dado** un Administrador/Ayudante **Y** una categoría "Escolares" que existe en el sistema
    + **Cuando** se selecciona la categoría "Escolares", se presiona "Eliminar categoría" y se confirma la operación.
    + **Entonces** el sistema elimina la categoría, pausa todas las publicaciones referidas a dicha categoría e informa en pantalla el mensaje "Categoría eliminada exitosamente".
- **Escenario 2: Eliminar Categoría exitoso**
    + **Dado** un Administrador/Ayudante **Y** no hay categorias cargadas en el sistema
    + **Cuando** se presiona "Eliminar categoría".
    + **Entonces** el sistema informa "Seleccione una categoría".
- **Escenario 3: Eliminar Categoría fallido cancelación de operación.**
    + **Dado** un Administrador/Ayudante **Y** una categoría "Escolares" que existe en el sistema.
    + **Cuando** selecciona la categoría "Escolares", presiona "Eliminar categoría" y cancela la operación.
    + **Entonces** el sistema muestra la pantalla previa a la solicitud de confirmación.
