# DulcesAdopciones

## Lista de entidades

### gato **(ED)**

- cat_id **(PK)**
- nombre
- edad
- raza
- color
- genero_id **(FK)**
- estado_salud
- imagenes
- historial_id **(FK)**
- esta_adoptado

### genero **(ED)**

- genero_id **(FK)**
- tipo

### direccion_casa **(ED)**

- direccion_id **(PK)**
- numero_casa **(UK)**
- calle_transversal
- parroquia
- sector
- provincia

### donante **(ED)**

- donante_id **(PK)**
- nombres
- apellidos
- numero_telefono
- direccion_id **(FK)**
- motivo_adopcion
- cat_id
- observaciones_mascotas

### historial_medico

- historial_id **(PK)**
- vacunas
- desparasitacion
- esterilizacion
- enfermedades

### condiciones_adopcion

- condiciones_id
- requisitos

## Relaciones

1. Un **genero** pertenece a un **gato**
2. Un **gato** tiene un **historial_medico**
3. Un **donante** da en adopcion a un/os **gato**
4. Un **donante** tiene una **casa**
5. Un **donante** tiene **condiciones_adopcion**

## Diagramas

## Reglas de Negocio

## Gato

1. Crear el registro de un **gato**
2. Leer el registro de un(os) gato(s) dada una condición en particular
3. Leer todos los registros de la entidad gato.
4. Actualizar los datos de un gato dada una condición en particular.
5. Eliminar los datos de un(os) gatos en caso de que ya sean adoptados

## direccion_casa

1. Crear el registro de una **direccion**
2. Leer el registro de una direccion dada una condición en particular
3. Leer todos los registros de la entidad direccion_casa.
4. Actualizar los datos de una direccion dada una condición en particular.

## donante

1. Crear el registro de un **donante**
2. Leer el registro de un(os) donante(s) dada una condición en particular
3. Leer todos los registros de la entidad donante.
4. Actualizar los datos de un donante dada una condición en particular.
5. Eliminar los datos de un(os) donante en caso de que ya sean adoptados

## historial_medico

1. Crear el registro de un **historial_medico**
2. Leer el registro de un historial dada una condición en particular
3. Leer todos los registros de un historial_medico.
4. Actualizar los datos de un historial_medico dada una condición en particular.
5. Eliminar los datos de un historial_medico
