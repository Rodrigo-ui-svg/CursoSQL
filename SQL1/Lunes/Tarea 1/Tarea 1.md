# Tarea 1

**Rodrigo Chávez de la Vega,** 
Hecho desde mysql- workbench
Teniendo el siguiente modelo:

![2](2.PNG)



- **Obtener el código para la creación de la tabla:**

  *Copiar el código en el bloque correspondiente*

  ```
  #Crear tabla, una vez ya creada la bd
CREATE TABLE CURSO(
    CURSO_ID NUMERIC(20,0) PRIMARY KEY NOT NULL,
    NOMBRE VARCHAR(40) NOT NULL,
    INSTRUCTOR_TITULAR VARCHAR(40) NOT NULL,
    INSTRUCTOR_ADJUNTO VARCHAR(40)  NULL,
    INSTRUCTOR_AUXILIAR VARCHAR(40) NULL,
    FECHA_INICIO DATE,
    FECHA_FIN DATE
);

#Instertar valores
INSERT INTO CURSO
 VALUES ("1", "Jorge", "Pedro", "Juan","J" , "1996-12-28", "2020-01-14" );
 INSERT INTO CURSO
 VALUES ("2", "Rodrigo", "Maria", "Jose", "I" , "1997-12-28", "2021-01-14" );
 INSERT INTO CURSO
 VALUES ("3", "Paulina", "Estela", "John","Ye" ,"1995-12-28", "2022-01-14" );
 INSERT INTO CURSO
 VALUES ("4", "Daniela", "Dana", "Manuel", "yo" ,"1996-11-28", "2020-11-14" );
 INSERT INTO CURSO
 VALUES ("5", "Jor", "Ped", "Ju","Santa Claus" ,"1993-12-28", "2026-01-14" );
 
 #Modificar la tabla CURSO en la columna NOMBRE por el nombre NOMBRE_CURSO
ALTER TABLE CURSO
Change NOMBRE NOMBRE_CURSO VARCHAR(40);


# Modificar la tabla *CURSO*, para agregar la columna *SEMESTRE*, que debe ser de tipo *VARCHAR2(20)
ALTER TABLE CURSO
ADD COLUMN SEMESTRE VARCHAR(15) AFTER FECHA_FIN;

#Modificar la tabla *CURSO*, para agregar la columna *Calificación*, que debe ser de tipo *NUMERIC(20)
ALTER TABLE CURSO
ADD COLUMN CALIFICACION NUMERIC(20,2) AFTER SEMESTRE;


#Modificar tabla *CURSO*, para eliminar la columna *FECHA_FIN***
ALTER TABLE CURSO
DROP FECHA_FIN;

#Modificar la tabla *CURSO* y renombrarla con el nombre *CURSO_INTERSEMESTRAL***
RENAME TABLE CURSO TO CURSO_INTERSEMESTRAL;

#Describe columnas
DESC CURSO_INTERSEMESTRAL;



#Actualizar la calificación del  curso cuyo *CURSO_ID* = 1, a *CALIFICACION*=10**
UPDATE CURSO_INTERSEMESTRAL 
SET 
    CALIFICACION = '10'
WHERE
 CURSO_ID = 1;


#Actualizar la calificación del  curso cuyo *CURSO_ID* = 2, a *CALIFICACION*=8.5**
UPDATE CURSO_INTERSEMESTRAL 
SET 
    CALIFICACION = '8.5'
WHERE
 CURSO_ID = 2;

 
 #Soltar la tabLA
 DROP TABLE CURSO;
 DROP TABLE CURSO_INTERSEMESTRAL;
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Llenar la tabla con por lo menos 5 Cargas (Es decir 5 datos a cada uno de los campos de la tabla)**

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Modificar la tabla *CURSO* en la columna *NOMBRE* por el nombre *NOMBRE_CURSO***

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Modificar la tabla *CURSO*, para agregar la columna *SEMESTRE*, que debe ser de tipo *VARCHAR2(20)***

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Modificar la tabla *CURSO*, para agregar la columna *Calificación*, que debe ser de tipo *NUMERIC(20)***

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Modificar tabla *CURSO*, para eliminar la columna *FECHA_FIN***

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Modificar la tabla *CURSO* y renombrarla con el nombre *CURSO_INTERSEMESTRAL***

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Actualizar la calificación del  curso cuyo *CURSO_ID* = 1, a *CALIFICACION*=10**

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

  

- **Actualizar la calificación del  curso cuyo *CURSO_ID* = 2, a *CALIFICACION*=8.5**

  *Copiar el código en el bloque correspondiente*

  ```sql
  
  ```

  *Pegar la captura de pantalla de la creación exitosa del código puesto anteriormente*

