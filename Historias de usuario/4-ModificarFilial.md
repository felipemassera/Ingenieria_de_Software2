## Título:
Modificar Filial

## Narrativa:
- Como Administrador
- Quiero modificar una filial
- Para actualizar los datos en el sistema

## Reglas de Negocio
    - El nombre de la filial no se puede repetir
    - Un unico ayudante responsable por filial.
## Criterios de aceptación:
- **Escenario 1: Modificar el nombre de filial exitoso**
    + **Dado** un Administrador **Y** un nombre "filial 520" que no esta registrado en el sistema. 
    + **Cuando** se modifica el nombre de la filial "filial 44" a "filial 520", se presiona "Modificar filial" y se confirma la operación.
    + **Entonces** el sistema modifica la filial e informa en pantalla "Filial modificada exitosamente"

- **Escenario 2: Modificar el ayudante de filial exitoso**
    + **Dado** un Administrador **Y** un ayudante DNI "44502629" que no es responsable de una filial. 
    + **Cuando** se selecciona el ayudante DNI "44502629", se presiona "Modificar filial" y se confirma la operación.
    + **Entonces** el sistema modifica la filial e informa en pantalla "Filial modificada exitosamente"

- **Escenario 3: Modificar el nombre de filial fallido, nombre de sucursal repetido**
    + **Dado** un Administrador **Y** un nombre "filial 44" que esta registrado en el sistema.
    + **Cuando** se modifica el nombre de la filial "filial 520" a "filial 44", se presiona "Modificar filial" y se confirma la operación.
    + **Entonces** el sistema informa en pantalla "El nombre de la filial ya se encuentra registrado".

- **Escenario 4: Modificar el ayudante de filial fallido, el ayudante ya se encuentra como responsable de otra filial**
    + **Dado** un Administrador **Y** un ayudante DNI "34987521" que es responsable de una filial. 
    + **Cuando** se selecciona el ayudante DNI "34987521", se presiona "Modificar filial" y se confirma la operación.
    + **Entonces** el sistema informa en pantalla "El ayudante se encuentra como responsable de otra filial".

**Escenario 5: Modificar filial fallido se cancela la operacion**
    + **Dado** un Administrador, un nombre "filial 520", que no esta registrado en el sistema **Y** un ayudante DNI "44502629" que no es responsable de una filial.
    + **Cuando** se modifica el nombre de la filial "filial 44" a "filial 520", se selecciona el ayudante DNI "44502629", se presiona "Modificar filial" y se cancela la operación.
    + **Entonces** el sistema cancela la operación y retorna a la pantalla anterior a la solicitud de confirmación.    