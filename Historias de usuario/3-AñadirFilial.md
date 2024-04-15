## Título:
Añadir Filial

## Narrativa:
- Como Administrador
- Quiero añadir una filial
- Para actualizar los datos en el sistema

## Reglas de Negocio
    - El nombre de la filial no se puede repetir
    - Un unico ayudante responsable por filial.
## Criterios de aceptación:
- **Escenario 1: Agregar filial exitoso**
    + **Dado** un Administrador, un nombre "filial 44", que no esta registrado en el sistema **Y** un ayudante DNI "44502629" que no se encuentra como responsable en otra filial. 
    + **Cuando** se ingresa el nombre de la filial "filial 44", la dirección "calle 44 esquina 23 numero 1234", se selecciona DNI "44502629" como ayudante para ser encargado de la sucursal, se presiona "Crear filial" y se confirma la operación.
    + **Entonces** el sistema crea la filial e informa en pantalla "Filial creada exitosamente"
    
    //CONSULTAR EL TEMA DEL AYUDANTE>.- 
    
    **Escenario 2: Agregar filial fallido, se cancela la operacion**
    + **Dado** un Administrador un nombre "filial 44", que no esta registrado en el sistema **Y** un ayudante DNI "44502629" que no se encuentra como responsable en otra filial. 
    + **Cuando** se ingresa el nombre de la filial "filial 44", la dirección "calle 44 esquina 23 numero 1234", se selecciona DNI "44502629" como ayudante para ser encargado de la sucursal, se presiona "Crear filial" y se cancela la operación.
    + **Entonces** el sistema cancela la operacion y retorna a la pantalla anterior a la solicitud de confirmación.
    - **Escenario 3: Agregar filial fallido nombre de filial repetido**
    + **Dado** un Administrador, un nombre "filial 44", que esta registrado en el sistema **Y** un ayudante DNI "44502629" que no se encuentra como responsable en otra filial. 
    + **Cuando** se ingresa el nombre de la filial "filial 44", la dirección "calle 44 esquina 23 numero 1234", se selecciona DNI "44502629" como ayudante encargado de la sucursal y se presiona "Crear filial" y confirma la operación.
    + **Entonces** el sistema informa en pantalla "El nombre de la filial ya se encuentra registrado"
    - **Escenario 4: Agregar filial fallido el ayudante ya se encuentra asignado a otra filial**
    + **Dado** un Administrador, un nombre "filial 520", que no esta registrado en el sistema **Y** un ayudante DNI "44502629" que se encuentra como responsable en otra filial. 
    + **Cuando** se ingresa el nombre de la filial "filial 44", la dirección "calle 44 esquina 23 numero 1234", se selecciona el ayudante DNI "44502629" como encargado de la sucursal y se presiona "Crear filial" y confirma la operación.
    + **Entonces** el sistema informa en pantalla "El ayudante ya se encuentra asignado a otra sucursal".