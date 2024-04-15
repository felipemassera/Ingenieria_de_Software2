## Título:
Eliminar Filial

## Narrativa:
- Como Administrador
- Quiero eliminar una filial
- Para actualizar los datos en el sistema

## Reglas de Negocio

## Criterios de aceptación:
- **Escenario 1: Eliminar filial exitoso**
    + **Dado** un Administrador **Y** una  filial "Filial 44". 
    + **Cuando** se selecciona la filial "filial 44", se presiona "Eliminar filial" y se confirma la operación.
    + **Entonces** el sistema elimina la filial e informa en pantalla "Filial eliminada exitosamente".

- **Escenario 2: Eliminar filial fallido, se cancela la confirmación**
    + **Dado** un Administrador **Y** una  filial "Filial 44". 
    + **Cuando** se selecciona la filial "filial 44", se presiona "Eliminar filial" y se cancela la operación.
    + **Entonces** el sistema cancela la operación y retorna a la pantalla anterior a la solicitud de confirmación.