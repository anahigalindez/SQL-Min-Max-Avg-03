# Actividad:

1. Crear una Base de datos en MySql llamada: Biblioteca.
2. Crear una tabla llamada **Autores** que contenga los campos de la tabla.
3. Realizar CRUD para que la tabla tenga los siguientes datos:

```
INSERT INTO `autores`
VALUES  ('Gabriel', 'García Márquez', '1927-03-06', 'Colombiano', 'Cien años de soledad', 1967, 40),
        ('Julio', 'Cortázar', '1914-08-26', 'Argentino', 'Rayuela', 1963, 48),
        ('Mario', 'Vargas Llosa', '1936-03-28', 'Peruano', 'La ciudad y los perros', 1963, 26),
        ('Pablo', 'Neruda', '1904-07-12', 'Chileno', 'Veinte poemas de amor y una canción desesperada', 1924, 19),
        ('Isabel', 'Allende', '1942-08-02', 'Chilena', 'La casa de los espíritus', 1982, 40),
        ('Jorge Luis', 'Borges', '1899-08-24', 'Argentino', 'Ficciones', 1944, 45),
        ('Octavio', 'Paz', '1914-03-31', 'Mexicano', 'El laberinto de la soledad', 1950, 36),
        ('Clarice', 'Lispector', '1920-12-10', 'Brasileña', 'La hora de la estrella', 1977, 56),
        ('Juan', 'Rulfo', '1917-05-16', 'Mexicano', 'Pedro Páramo', 1955, 38),
        ('Carlos', 'Fuentes', '1928-11-11', 'Mexicano', 'La región más transparente', 1958, 29),
        ('Eduardo', 'Galeano', '1940-09-03', 'Uruguayo', 'Las venas abiertas de América Latina', 1971, 31);

```

4. Realizar las siguientes consultas:
  
### Listar todos los autores de que sean de nacionalidad argentina.

```
SELECT * FROM `Autores` WHERE `Nacionalidad` LIKE "Argentin%";
```

### Listar todos los autores que hayan publicado entre 1960 a 1980.

```
SELECT * FROM `autores` WHERE `Año de publicación` BETWEEN 1960 AND 1980;
```

### Mostrar el promedio de la edad de publicación (avg).

```
SELECT AVG(`Edad de Publicación`) FROM `Autores`;
```
