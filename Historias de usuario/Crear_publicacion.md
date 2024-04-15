Eliminar publicación.
Pausar publicación.
Mostrar mapa. //landing page
Acceder al e-commerce. 
Intercambiar puntos. 
Enviar solicitud de intercambio.
Aceptar o rechazar intercambio. //entonces Enviar identificador de intercambio

## Título:
Crear publicacion

## Narrativa:
- Como usuario registrado
- Quiero crear publicaciones
- Para realizar intercambios con otros usuarios

## Reglas de Negocio
- Maximo de 5 publicaciones
- Debe de tener una descripcion
- Debe de tener su categoria de producto

## Criterios de aceptación:
- **Escenario 1: Crear publicacion exitoso**
    + **Dado** un usuario registrado con un titulo "Quesitas", una descripcion "Son quesitas", la categoria "comida" **Y** tiene 4 publicaciones activas
    + **Cuando** ingresa el titulo "Quesitas", la descripcion "Son quesitas", selecciona la categoria "comida" y presiona "Subir publicacion"
    + **Entonces** el sistema sube exitosamente la publicacion y se informa en pantalla el mensaje "Publicacion subida exitosamente"
- **Escenario 2: Crear publicacion fallido por limite de publicaciones**
    + **Dado** un usuario registrado con un titulo "Quesitas", una descripcion "Son quesitas", selecciona la categoria "comida" **Y** tiene 5 publicaciones activas
    + **Cuando** ingresa el titulo "Quesitas", la descripcion "Son quesitas", la categoria "comida" y presiona "Subir publicacion"
    + **Entonces** el sistema informa informa en pantalla el mensaje "Limite de publicaciones alcanzado"
- **Escenario 3: Crear publicacion fallido por falta de descripcion**
    + **Dado** un usuario registrado con un titulo "Quesitas", sin una descripcion, la categoria "comida" **Y** tiene 4 publicaciones activas
    + **Cuando** ingresa el titulo "Quesitas", selecciona la categoria "comida" y presiona "Subir publicacion"
    + **Entonces** el sistema informa informa en pantalla el mensaje "Ingresar la descripcion de la publicacion, por favor"
- **Escenario 4: Crear publicacion fallido por falta de categoria**
    + **Dado** un usuario registrado con un titulo "Quesitas", una descripcion "Son quesitas", sin una categoria **Y** tiene 4 publicaciones activas
    + **Cuando** ingresa el titulo "Quesitas", la descripcion "Son quesitas" y presiona "Subir publicacion"
    + **Entonces** el sistema informa en pantalla el mensaje "Seleccionar la categoria de la publicacion, por favor"
- **Escenario 5: Crear publicacion fallido por falta de titulo**
    + **Dado** un usuario registrado sin un titulo, con una descripcion "Son quesitas", la categoria "comida" **Y** tiene 4 publicaciones activas
    + **Cuando** ingresa la descripcion "Son quesitas", selecciona la categoria "comida" y presiona "Subir publicacion"
    + **Entonces** el sistema informa en pantalla el mensaje "Ingresar el titulo de la publicacion, por favor"