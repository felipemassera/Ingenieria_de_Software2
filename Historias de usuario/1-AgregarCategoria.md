## Título:
Agregar categoría

## Narrativa:
- Como Administrador/Ayudante
- Quiero crear categoría
- Para organizar el listado de productos

## Reglas de Negocio

## Criterios de aceptación:
- **Escenario 1: Agregar Categoria exitoso**
    + **Dado** un Administrador/Ayudante **Y** una categoría "Escolares" que no existe en el sistema.
    + **Cuando** se ingresa el nombre de la categoría "Escolares", se presiona "Crear categoría" y se confirma la operación.
    + **Entonces** el sistema crea la categoría e informa en pantalla el mensaje "Categoria creada exitosamente"
- **Escenario 2: Agregar Categoria fallido, cancelación de operación.**
    + **Dado** un Administrador/Ayudante **Y** una categoría "Escolares" que no existe en el sistema.
    + **Cuando** se ingresa el nombre de la categoría "Escolares", se presiona "Crear categoría" y se cancela la operación.
    + **Entonces** el sistema muestra la pantalla previa a la solicitud de confirmación. 
- **Escenario 3: Agregar Categoria fallido, categoría ya existente**
    + **Dado** un Administrador/Ayudante **Y** una categoría "Escolares" que ya existe en el sistema.
    + **Cuando** se ingresa el nombre de la categoría "Escolares", se presiona "Crear categoría" y se confirma la operación.
    + **Entonces** el sistema informa  "La categoría ya existe en el sistema".