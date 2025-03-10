# Ejercicios
Acá se subirán todos los ejercicios correspondientes a las unidades del Laboratorio de Programación Orientado a Objetos 2025.

## Repaso estructuras en C++

1. Crear la estructura `Empleado` que tiene un nombre, apellido, fecha de nacimiento, sexo y salario.  

   Se pide la función `empleadoConMayorSueldo` que recibe por parámetro un vector con todos los empleados de la empresa y otro vector vacío donde se guardarán los empleados que tienen salario menor o igual a $400.000.  

   La función deberá recorrer todos los empleados de la empresa y retornar el de mayor sueldo. Además, a medida que va recorriendo los empleados, debe agregar al otro vector los empleados cuyo salario es menor o igual a $400.000.  

   Por lo tanto, luego de llamar a la función, se quiere mostrar en el `main` el empleado con mayor sueldo y mostrar el nombre y apellido de todos los empleados con salario menor o igual a $400.000.  

2. Se quieren almacenar los productos de un supermercado. De estos interesa conocer el nombre, código de barra, marca, precio y si tiene fecha de vencimiento o no.  

   Los pasillos del supermercado están compuestos por góndolas de 3 filas y 4 columnas. Ingresar tantos productos como sea necesario para llenar un pasillo y determinar:  

   - Columna de la góndola que tiene el precio de mayor valor.  

   - Nombre del producto de la fila 2, columna 3.  

   - Promedio de precios de todo ese pasillo.  

   - Cantidad de productos con fecha de vencimiento.

3. Se quiere hacer un sistema de gestión de pedidos de un Restaurante. Cada pedido tiene un número de pedido, el nombre del cliente, una lista de productos, cantidades y precios. El sistema debe permitir:
   - Agregar un nuevo pedido con sus productos.
     
   - Cancelar un pedido buscando por el número de pedido.
     
   - Mostrar todos los pedidos en curso con el total de cada uno.
     
   - Calcular el ingreso total del día sumando los totales de todos los
pedidos completados.

4. Se quiere hacer un sistema de gestión de pacientes en una clínica. Cada paciente tiene los siguientes datos: nombre, edad, número de historia clínica, y fecha de próxima cita (día, mes y año como una estructura de tipo Fecha). El sistema debe permitir:
   - Registrar nuevos pacientes y asignarles una fecha de cita.
     
   - Cancelar una cita buscando al paciente por número de historia clínica.
     
   - Mostrar todas las citas programadas para un día específico.
     
   - Buscar y mostrar información de un paciente usando su número
de historia clínica.
   
5. Realizar un sistema para la gestión de un McDonald’s. El sistema cuenta con un menú de 20 productos diferentes, cada uno esta conformado por: Un nombre, si tiene promoción o no, cantidad de ventas, el precio y la categoría a la que pertenece (Hamburguesa, Bebida, Postre, etc.). Ademas, cada pedido realizado debe registrar los siguientes datos: El nombre del cliente, productos pedidos, cantidad de cada producto, la fecha que se pidió y el precio total.
   
   #### Requerimientos:
   - Se deberá implementar al menos 2 estructuras y 4 funciones.
     
   #### Funcionalidades:
   - El usuario, antes de poder realizar cualquier acción en el sistema, deberá ingresar todos los productos al mismo.
     
   - Luego de cargar los productos al sistema, el usuario deberá poder registrar un pedido, calculando automáticamente el precio total, considerando las promociones activas (Para los productos que tienen promociones activas, se les aplicará un descuento del 20% al precio del producto).
     
   - El usuario deberá poder consultar un pedido específico por el nombre del cliente. Mostrando por pantalla la información del pedido.
     
   - El sistema deberá mostrar por pantalla los productos ordenados por ventas de mayor a menor.

6. Realizar un sistema para la organización de un torneo de futbol. El torneo está compuesto por 24 equipos, cada uno está conformado por: un nombre, 11 jugadores (1 jugador es el arquero), la cantidad de goles a favor y en contra, la posición en el torneo (Determinada por los resultados de los partidos: Las Victorias suman : +3, los Empates suman: +1 y las Derrotas suman: +0) y el historial de partidos (Se guardará en formato: V, E, D).

   Ademas, cada partido debe registrar los siguientes datos: El nombre de los equipos (Local y Visitante), cantidad de goles anotados por cada equipo, la fecha y el estadio donde se disputó.

   #### Requerimientos:
   - Se deberá implementar al menos 3 estructuras y 4 funciones.

   #### Funcionalidades:
   - El usuario deberá poder ingresar todos los equipos al sistema.
     
   - El usuario deberá poder registrar todos los datos de cada partido, actualizando la información de los equipos que jugaron.
     
   - El usuario deberá poder mostrar por pantalla, la información de un partido especifico, seleccionando los nombres de los equipos que se enfrentaron.
     
   - El usuario deberá poder mostrar la tabla de posiciones del torneo, ordenada de mayor a menor según la puntuación. En caso de empate en la puntuación, el desempate se realizara en base a la Cantidad de goles a favor (De mayor a menor). La tabla debe mortrar: Posición - Nombre del equipo - Cantidad de goles a favor - Cantidad de goles en contra - Historial de partidos.

7. Realizar un sistema para la organización de carreras de Formula 1. En total se corren 24 carreras por año y están compuestas por 10 equipos, cada uno esta conformado por 2 pilotos (Por lo que serán 20 pilotos en total), se deberá hacer un sistema para determinar el equipo ganador anual de Formula 1.
   
      #### Estructuras:
      - Cada piloto está conformado por: un nombre, el numero del auto, el nombre del equipo que participan, la posición que arrancan la carrera, la posición en la que la finalizan, la cantidad de puntos que obtuvieron por carrera (Los primeros 10 puestos suman puntaje) y si obtuvo la vuelta rápida o no.
      - 
      ~~~
         struct Vuelta_rapida {
           int numero_vuelta;
           int tiempo;
           string nombre_piloto;
         }
      
         struct Equipo {
            string nombre;
            int puntos;
         }
      ~~~
        
      #### Funcionalidades:
      Utilizando el siguiente main (Pueden agregar más variables y funciones, elegir el tipo de dato de las funciones, como devuelven su info. y los parámetros de las mismas), deberán hacer todo lo que se pide en cada punto, tengan en cuenta que los equipos ya tienen su nombre y se encuentran con 0 puntos.
   
      ~~~
      int main(){
         vector<Equipo> equipos;
         vector<Piloto> pilotos;
         for (int i = 0; i < 24; i++){
            // 1
            cargar_datos_carrera();
            // 2
            calcular_puntaje_piloto_equipo();
         }
         // 3
         ordenar_tabla_equipos();
         mostrar_tabla_equipos();
      }
      ~~~
      
      1- Cargar los pilotos por posición de llegada en la carrera y quien hizo la vuelta rápida.
         
      2- Calcular en base a la posición de llegada, los puntos que suman los pilotos a su equipo (Los
      puntos van del primer al décimo puesto: 25, 18, 15, 12, 10, 8, 6, 4, 2 y 1 puntos). Tener en
      cuenta la vuelta rápida (La vuelta rápida suma 1 punto adicional, si el piloto se encuentra en
      los primeros 10 puestos).
      
      3- Ordenar y mostrar por pantalla, la tabla de mayor a menor puntaje para saber el equipo
      ganador anual de Formula 1.
