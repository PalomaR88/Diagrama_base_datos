# Diagrama de base datos
### [Ejercicios prácticos](https://github.com/PalomaR88/Diagrama_base_datos/tree/master/Boletin_2)
#### Autoescuela
En una autoescuela hay varios profesores y varios coches de prácticas. Se requiere guardar información respecto a los alumnos que se matriculan, el profesor que se le asigna y el coche que conducirán.
Cada alumno da clase con un profesor en un coche. El alumno siempre va a conducir el mismo coche para habituarse a él y va a dar clase con el mismo profesor. 
Si un día un profesor no puede dar clase, el alumno puede cambiar de profesor aunque no de coche. ¿Cómo afectaría esta nueva situación?
[Ejercicio en xml](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/Boletin_2/3.xml)
![img3](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/images/3.png)

#### Banco
En un banco se tienen varias sucursales. Un cliente puede ir a cualquier sucursal y abrir una cuenta. En realidad, el cliente puede abrir varias cuentas en la misma o distinta sucursal. Una cuenta puede pertenecer a uno o varios clientes.
Sobre una determinada cuenta, se pueden realizar varias transacciones.
Cada sucursal viene identificada por un número de sucursal, también interesa conocer la ciudad en la que se encuentra ubicada y el activo disponible.
Por su parte, cada cuenta tiene asociado un número de cuenta y saldo.
Del cliente, interesa almacenar el DNI, el nombre, la dirección y la ciudad en la que
reside.
Cada transacción que se realiza sobre una cuenta tiene un número (de transacción) diferente. Además, se marca la fecha del día, el tipo de operación que se realiza (Ingreso/Extracción) y la cantidad que se mueve.
[Ejercicio en xml](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/Boletin_2/4.xml)
![img4](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/images/4.png)

#### Municipios/viviendas/personas
Supongamos el siguiente universo del discurso sobre municipios, viviendas y personas.
Cada persona sólo puede habitar en una vivienda y estar empadronada en un municipio, pero puede ser propietaria de varias viviendas. Nos interesa también conocer las personas que dependen del Cabeza de Familia (C.F.). Se indicarán lossupuestos semánticos que se consideren oportunos para justificar todas las decisiones de diseño.
[Ejercicio en xml](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/Boletin_2/6.xml)
![img6](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/images/5.png)

#### Departamento de formación
El departamento de formación de una empresa desea construir una base de datos para planificar y gestionar la formación de sus empleados.
La empresa organiza cursos internos de formación de los que se desea conocer el código de curso, el nombre, una descripción, el número de horas de duración y el coste del curso.
Un curso puede tener como prerrequisito haber realizado otro(s) previamente, y, a su vez la realización de un curso puede ser prerrequisito de otros. Un curso que es un prerrequisito de otro puede serlo de forma obligatoria o sólo recomendable.
Un mismo curso tiene diferentes ediciones, es decir, se imparte en diferentes lugares, fechas y con diferentes horarios (intensivo, de mañana o de tarde). En una misma fecha de inicio sólo puede impartirse una edición de un curso.
Los cursos se imparten por personal de la propia empresa.
De los empleados se desea almacenar su código de empleado, nombre y apellidos, dirección, teléfono, NIF (Número de Identificación Fiscal), fecha de nacimiento, nacionalidad, sexo, firma y salario, así como si está o no capacitado para impartir cursos.
Un mismo empleado puede ser docente en una edición de un curso y alumno en otra edición, pero nunca puede ser ambas cosas a la vez (en una misma edición de curso o lo imparte o lo recibe).
[Ejercicio en xml](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/Boletin_2/7.xml)
![img7](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/images/7.png)

#### Auditorio Municipal
El Auditorio Municipal Alfredo Kraus desea crear un sistema de reservas, para lo cual es necesario en primer lugar, crear una base de datos que almacene toda la información de los conciertos que organiza. Los conciertos se organizan por temporadas. Cada año consta de tres temporadas: Verano, Otoño/Invierno y Primavera. Cada concierto sólo puede pertenecer a una única temporada y se celebrará en una fecha determinada a una hora determinada. También hay que almacenar el título del concierto y su duración aproximada.
En los conciertos intervienen uno o varios intérpretes que pueden ser de tres tipos: músicos con carácter individual, grupos (dúos, tríos, cuartetos,...) o bien orquestas.
En el caso de músicos individuales, interesa almacenar el instrumento que toca, su nombre y un breve curriculum. Para grupos hay que indicar si son dúos, tríos, cuartetos, etc., el nombre del grupo y un curriculum del grupo. Además interesa el nombre de cada uno de sus componentes (músicos) así como el instrumento que tocan. En este sentido es importante tener en cuenta que todos los músicos que pertenecen a un grupo deben considerarse también músicos individuales. Sin embargo, no todos los músicos "individuales" tienen porqué pertenecer a grupos.
Finalmente, en el caso de orquestas sólo interesa saber el nombre de la orquesta, el
número de músicos que lo componen, el nombre del director y un curriculum de dicha orquesta.
Cada concierto consta de un programa, formado por las piezas musicales de determinados autores.
Finalmente se quiere almacenar información sobre las entradas: número de entrada (único), el precio, que puede ser precio normal o reducido (jóvenes y tercera edad) y depende del concierto, la fila y número de asiento al que se corresponde dicha entrada, así como la fecha, hora y título del concierto. El número máximo de entradas es 150. No puede haber dos entradas con el mismo número de fila y asiento para un mismo concierto.
[Ejercicio en xml](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/Boletin_2/12.xml)
![img12](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/images/12.png)

#### Farmacia
La gestión de una farmacia requiere poder llevar control de los medicamentos existentes, así como de los que se van sirviendo, para lo cual se pretende diseñar un sistema acorde a las siguientes especificaciones:
En la farmacia se requiere una catalogación de todos los medicamentos existentes, para lo cual se almacenará un código de medicamento, nombre del medicamento, tipo de medicamento (jarabe, comprimido, pomada, etc.), unidades en stock, unidades vendidas y precio. Existen medicamentos de venta libre, y otros que sólo pueden dispensarse con receta médica.
La farmacia adquiere cada medicamento a un laboratorio, o bien los fabrica ella misma. Se desea conocer el código del laboratorio, nombre, teléfono, dirección, fax así como el nombre de la persona de contacto. Los medicamentos se agrupan en familias, dependiendo del tipo de enfermedades a las que dicho medicamento se aplica.
La farmacia tiene algunos clientes que realizan los pagos de sus pedidos a fin de cada mes (clientes con crédito). La farmacia quiere conocer las unidades de cada medicamento comprado (con o sin crédito) así como la fecha de compra. Además, es necesario tener los datos bancarios de los clientes con crédito, así como la fecha de pago de las compras que realizan.
[Ejercicio en xml](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/Boletin_2/14.xml)
![img14](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/images/14.png)

#### Almacenes
El departamento de almacenes de un supermercado necesita desarrollar una base de datos con información relativa a sus operaciones y funcionamiento interno.
Lo primero que se quiere guardar es la información relativa a clientes. Cada cliente viene identificado por un código. Además se tiene su nombre, dirección y teléfono de contacto.
Otro aspecto importante es la información de proveedores. De los proveedores interesa su nombre, sector productivo, antigüedad y ciudad en la que operan. Cada proveedor tiene un no de proveedor.
Por otro lado están los productos. Cada producto viene descrito por su código, nombre y precio unitario. Cada producto lo sirve un único proveedor.
De los pedidos se almacena la fecha de petición, la fecha de servicio y el importe total. Cada pedido está formado por un conjunto de productos, de cada uno de los cuales se pide una cantidad de unidades determinada. Cada pedido lo hace un único cliente.
[Ejercicio en xml](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/Boletin_2/15.xml)
![img15](https://github.com/PalomaR88/Diagrama_base_datos/blob/master/images/15.png)

![]()
![]()
![]()

