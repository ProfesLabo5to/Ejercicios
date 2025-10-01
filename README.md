

  
# Ejercicios
Acá se subirán todos los ejercicios correspondientes a las unidades del Laboratorio de Programación Orientado a Objetos 2025.

<details markdown="block">
<summary><strong>Unidad 0 – Introducción y repaso al laboratorio</strong></summary>

### 1. IngresoDatos
Escribe un programa en Java que realice lo siguiente:
- Declarar una variable `N` de tipo `int`
- Una variable `A` de tipo `double`
- Una variable `C` de tipo `char`

Luego de asignar a cada una un valor, mostrar por pantalla:
- El valor de cada variable.
- La suma de `N + A`
- La diferencia de `A – N`
- El valor numérico correspondiente al carácter que contiene la variable `C`.

Ejemplo de salida:

### 2. NumeroMayor
Declarar 2 variables numéricas e indicar cuál es mayor de los dos. En caso de que sean iguales, indicarlo también.

### 3. DivisibleFor / DivisibleWhile
Muestra los números del 1 al 100 (ambos incluidos) divisibles entre 2 y 3.

### 4. DiaLaboral
Crear un programa que nos pida un día de la semana y nos diga si es un día laboral o no. Los días laborales se consideran de lunes a viernes.

### 5. Vocales
Del siguiente String:  
`"Ayer me compré muñecos de la marca ‘ToyCo’ por internet."`  
Contar cuántas vocales hay en total y mostrarlo por pantalla.

### 6. ReemplazoLetra
Reemplazar todas las `e` del ejercicio anterior por la letra que ingrese el usuario.

### 7. IntroducirNumeros
Crear una aplicación que nos permite insertar números hasta que insertemos un `-1`. Luego, mostrar la cantidad de números introducidos.

### 8. IntroducirNumeros (Ampliado)
Al ejercicio anterior, además de la cantidad de números introducidos, se debe mostrar:
- Mayor número introducido.
- Menor número introducido.
- Suma de todos los números.
- Suma de los números positivos.
- Suma de los números negativos.

### 9. PalabrasIguales
Pedir dos palabras al usuario e indicar si son iguales o no.

</details>

<details markdown="block">
<summary><strong>Unidad 1 – Clases y objetos</strong></summary>

### 1. Clase `Círculo`
Crear una clase llamada `Círculo` con los siguientes atributos y métodos:
- Atributo: `radio`
- Constructor por defecto (`radio=2`)
- Constructor parametrizado
- Getter y setter
- Método para calcular el área (`π * r^2`)
- Método para calcular el perímetro (`2 * π * r`)

### 2. Clase `Rectángulo`
Crear una clase llamada `Rectángulo` con los siguientes atributos y métodos:
- Atributos: `base`, `altura`
- Constructor parametrizado
- Getters y setters
- Método para calcular el área
- Método para calcular el perímetro

### 3. Clase `Coche`
Crear una clase llamada `Coche` con los siguientes atributos y métodos:
- Atributos: `marca`, `modelo`, `color`
- Constructor parametrizado
- Getters y setters
- Métodos: `acelerar`, `frenar`, `mostrarVelocidadActual`

### 4. Clase `Persona`
Crear una clase llamada `Persona` con los siguientes atributos y métodos:
- Atributos: `nombre`, `edad`, `dirección`
- Método para imprimir los datos de la persona en pantalla

### 5. Clase `Fecha`
Crear una clase `Fecha` con los siguientes atributos y métodos:
- Atributos: `día`, `mes`, `año`
- Métodos:
  - `valida()`: Verifica si la fecha es correcta y ajusta valores inválidos.
  - `diasMes(int mes)`: Devuelve el número de días del mes indicado.
  - `corta()`: Muestra la fecha en formato corto (`dd-mm-yyyy`).
  - `larga()`: Muestra la fecha en formato largo (`día de la semana dd de mes de yyyy`).
  - `siguiente()`: Avanza un día.
  - `anterior()`: Retrocede un día.
  - `igualQue(Fecha fecha)`: Indica si la fecha es igual a otra.
  - `menorQue(Fecha fecha)`: Indica si la fecha es anterior a otra.
  - `mayorQue(Fecha fecha)`: Indica si la fecha es posterior a otra.

### 6. Clase `Libro`
Crear una clase llamada `Libro` con los siguientes atributos y métodos:
- Atributos: `título`, `autor` (usar la clase `Persona`), `ISBN`, `páginas`, `editorial`, `fechaPublicacion` (usar la clase `Fecha`)
- Métodos:
  - Mostrar la información del libro
  - Comparar si la fecha de publicación es anterior a otro libro dado
  - 3 constructores distintos a elección
  - Getters y setters

### 7. Clase `Cafetera`
Modelar una `Cafetera` con los siguientes atributos y métodos:
- Atributos: `cantidadMaxima`, `cantidadActual`
- Métodos:
  - `Constructor por defecto`: Cantidad máxima = 1000cc, cantidad actual = 0cc.
  - `Constructor con cantidad máxima`: Inicializa cantidad actual a la capacidad máxima.
  - `Constructor con cantidad máxima y actual`: Ajusta la cantidad actual si es mayor que la capacidad.
  - `llenarCafetera()`: Llena la cafetera al máximo.
  - `servirTaza(int capacidad)`: Sirve café en una taza hasta la capacidad indicada.
  - `vaciarCafetera()`: Vacía la cafetera.
  - `agregarCafe(int cantidad)`: Añade café a la cafetera.

### 8. Clase `Cancion`
Crear una clase llamada `Cancion` con los siguientes atributos y métodos:
- Atributos: `título`, `autor`
- Métodos:
  - Constructor por defecto (inicializa atributos con cadenas vacías)
  - Constructor parametrizado
  - Getters y setters

</details>

<!-- línea en blanco antes y después de cada bloque <details> -->
<details markdown="block">
<summary><strong> Unidad 2 - ArrayLists y for each</strong></summary>

### 1. Operaciones básicas con ArrayLists
En un programa:

a. Crear un `ArrayList` de números enteros y mostrar su suma.  
b. Crear un `ArrayList` de palabras y mostrar solo los elementos que empiezan con una letra específica.  
c. Crear un `ArrayList` de objetos `Persona` y mostrar solo las personas que tienen más de 30 años.

### 2. Clase `CD`
Crear una clase `CD` compuesta de muchas canciones e implementar los siguientes métodos:
- Constructor por defecto.
- Getters y setters.
- `numeroCanciones()`: Devuelve la cantidad de canciones en el CD.
- `verCancion(int posicion)`: Devuelve la canción que se encuentra en esa posición.
- `grabaCancion(int posicion, Cancion nuevaCancion)`: Reemplaza la canción en esa posición por una nueva.
- `agrega(Cancion cancion)`: Agrega una canción al final del `ArrayList`.
- `elimina(int posicion)`: Elimina la canción en la posición indicada.

### 3. Clase `Alumno` (básica)
Crear una clase que represente a un alumno de una escuela con los siguientes atributos:
- `nombre`, `apellido`, `fechaNacimiento`, `listaDeNotas`

Métodos:
- Getters y setters de todos los atributos.
- `agregarNota()`
- `menorNota()`
- `mayorNota()`

### 4. Clase `Alumno` con materias
Extensión del ejercicio anterior incorporando un atributo `materias`, el cual representa una lista de objetos `Materia`.

Clase `Materia`:
- Atributos: `nombre`, `listaDeContenidos`, `alumnosInscriptos`

Métodos sugeridos:
- `agregarMateria()`
- `promedioEdadAlumnos()`
- `promedioNotasAlumno()`

### 5. Sistema de campeonatos de Curling
Realizar un sistema que controle campeonatos de curling.

**Requisitos del sistema:**
- Los equipos deben registrarse con:
  - Nombre del equipo
  - Barrio de procedencia
  - 11 jugadores (uno de ellos marcado como capitán)
  - Disponibilidad horaria (mañana, tarde, noche)

**De cada jugador:**
- Nombre
- Fecha de nacimiento
- Número de camiseta (no se puede repetir dentro del mismo equipo)

**Reglas del torneo:**
- Modalidad todos contra todos
- El sistema debe generar el fixture completo
- Cada partido debe tener un día, turno y los equipos que juegan
- Los partidos se agendan según disponibilidad horaria de los equipos
</details>

<details markdown="block">
<summary><strong> Ejercicios repaso evaluación 12/05</strong></summary>

### 1. Sistema de videoclubs

Aparecieron de vuelta los videoclubs en la ciudad que se encargan de vender películas, ya sea en formato digital o físico. Nos han solicitado hacer el sistema que los administre.

Las películas que pertenecen al establecimiento guardan:
- Nombre
- Género
- Duración
- Director/es
- Actor/es
- Idiomas disponibles

Estas películas se organizan dentro de estanterías que se identifican con un número y guardan todas las películas que almacenan.

Cada videoclub guarda:
- Dirección
- Código postal
- Estanterías que contiene

Se solicita modelar las clases con sus atributos correspondientes, constructores, getters y setters. Además, realizar una clase de prueba para cumplir con las siguientes funcionalidades:

a) ABM de videoclubs, estanterías y películas.

b) Mostrar el nombre y estantería de la película con mayor duración de un videoclub.

c) Dada una película, retornar los actores mayores de edad.

d) Retornar los directores que estén en más de una película de una estantería.

e) Retornar las direcciones de los videoclubs que pertenezcan a una comuna en particular.

f) Mostrar las películas de duración menor a 90 minutos con ubicación.

g) Retornar el videoclub con más películas totales.

h) Dado un género, mostrar qué películas hay en cada videoclub registrado.


### 2. Clases necesarias para un `main`

Dada una clase `main`, hacer las clases necesarias (con sus respectivos atributos y métodos) para que funcione correctamente.


```java
public static void main(String[] args) {
    Persona p1 = new Persona("Miguel", "Lopez", 32987990,
        LocalDate.of(1985, 10, 12), LocalDate.of(2020, 5, 8));
    Persona p2 = new Persona("Juana", "Gomez", 39987990,
        LocalDate.of(1986, 7, 28));
    Persona p3 = new Persona("Candela", "Navarro", 40987990,
        LocalDate.of(1993, 2, 4), LocalDate.of(2017, 5, 25));

    BancoNacion sucursalUrquiza = new BancoNacion("Av. Triunvirato 3450", true, false);
    BancoNacion sucursalPueyrredon = new BancoNacion("Cochrane 2874", true, true);

    ArrayList<BancoNacion> sucursales = new ArrayList<>();

    sucursales.add(sucursalUrquiza);
    sucursales.add(sucursalPueyrredon);

    sucursalUrquiza.agregarTrabajador(p1);
    sucursalUrquiza.agregarTrabajador(p3);
    sucursalPueyrredon.agregarTrabajador(p2);

    sucursalPueyrredon.cantidadTrabajadores();

    for (BancoNacion b : sucursales) {
        Persona p = b.empleadoMayorAntiguedad();
        System.out.println(p.getNombre() + " " + p.antiguedad());
    }
}
```
</details>

<details markdown="block">
<summary><strong> Unidad 3 - Herencia</strong></summary>

### 1. Revisar ejercicios anteriores y detectar herencias  
Revisar los ejercicios anteriores y determinar dónde utilizar herencia (por ejemplo, entre `Rectángulo` y `Círculo`, o entre `Persona` y `Alumno`).  

*Aclaración:* Si es necesario modificar clases ya creadas, háganlo.

### 2. Sistema de flota de vehículos  
Realizar un sistema que maneje la flota de vehículos de una empresa. De todos los vehículos (autos, camionetas y bicicletas) se debe conocer su marca, modelo, color, cantidad de ruedas y año de fabricación. Para los autos y las camionetas, guardar además la patente; en las camionetas, la capacidad de carga en kg; y en los autos, si son descapotables o no.  
La empresa debe poder:  
- Saber de qué tipo de vehículo posee más cantidad  
- Añadir carga a una camioneta (sin superar su capacidad)  
- Conocer el porcentaje de autos descapotables.

### 3. Sistema de pedidos de almuerzos  
Realizar un sistema para la gestión de pedidos de almuerzos. Los pedidos pueden ser realizados por alumnos (nombre, apellido, división) o profesores (nombre, apellido, porcentaje de descuento). Los platos tienen nombre y precio. Al registrar un pedido, incluir fecha de creación, plato, solicitante, hora de entrega y estado de entrega. El sistema debe permitir agregar, modificar y eliminar platos, y mantener una lista de pedidos. Se solicita:  
- Listado de platos a cocinar en un día con su precio (aplicando descuentos)  
- Top 3 de platos más pedidos.
  
### 4. Compra de computadoras personalizadas  
Crear las clases necesarias para un sitio web de venta de computadoras personalizadas. El usuario elige una CPU y varios periféricos; la compra mínima incluye una CPU, un dispositivo de entrada y uno de salida. Al concretar la compra, guardar nombre, apellido, celular del cliente y método de pago (si es con tarjeta, 5 % de recargo y datos de la tarjeta).  
Todos los componentes incluyen fabricante, modelo, precio (ajustable por inflación) y stock.  
  -   **Entrada:** teclado y mouse (tipo de conector y puertos)  
  -   **Salida:** pantallas e impresoras (puertos; para impresoras, método de impresión: inyección o láser)
  
Debe admitirse la incorporación de nuevos periféricos.  
El programa deberá:  

- Agregar la compra a la lista de computadoras vendidas y actualizar stock  
- Calcular el precio total con todos los periféricos  
- Mostrar la cantidad de dispositivos de entrada y de salida de una computadora vendida específica.

### 5. Sistema de alarmas de edificio  
Un edificio dispone de detectores de humo, sensores de temperatura y sensores de presión. Cada dispositivo tiene estado (conectado/desconectado), medida (valor real), umbral inicial y año de adquisición (para mantenimiento). El sistema recorre continuamente los dispositivos conectados y toma medidas; si la medida supera el umbral, dispara la alarma:  
- Detector de humo: imprimir llamada a bomberos  
- Sensor de temperatura: imprimir “¡Cuidado! La temperatura sube”  
- Sensor de presión: imprimir “Sensor de presión activado”  
Para evitar falsas alarmas, varios dispositivos pueden agruparse; el sensor compuesto dispara la alarma si la suma de las medidas del grupo dividida entre 3 supera su umbral. 

### 6. Control de llamadas telefónicas  
Realizar un sistema que registre las llamadas entre empleados de una empresa. Cada empleado tiene nombre, apellido, DNI, país y teléfono. Para realizar una llamada, se introduce el número destino; al finalizar, se registra la duración. El sistema debe almacenar: empleado origen, empleado destino, fecha y duración de cada llamada, y debe ser capaz de generar un listado de llamadas por empleado y un ranking de empleados que más tiempo llamaron al exterior. 
</details>


<details markdown="block">
<summary><strong>Unidad 4 - Enums</strong></summary>

### 1. Editoriales válidas
Hacer que las únicas editoriales de los libros que se crean puedan ser:
- Kapelusz  
- Sudamericana  
- Atlántida  
- El Ateneo  
- Interzona  
- Sur  
- Alianza

### 2. Turnos en el ejercicio 5 de la Unidad 2
Realizar las modificaciones necesarias en el ejercicio 5 de la **Unidad 2** para que los únicos turnos posibles sean:
- Mañana  
- Tarde  
- Noche

### 3. Colores con códigos hexadecimales
Crear una clase `enum` donde se describan distintos colores junto a su código hexadecimal e implementarlo en las clases en las que pidan colores.

### 4. Aplicación de enums en ejercicios anteriores
¿En otros enunciados de los que ya hicimos podés modificar los valores para crear clases enumerables? Hacelo en todos los que puedas.

### 5. Tienda de productos electrónicos
En una tienda de electrónica venden distintos tipos de productos. Si bien todos tienen un nombre, precio y un stock, según en qué sección se encuentran son los datos que interesa almacenar. 
Los equipos de sonido, que pertenecen a la sección Multimedia, tienen un atributo para indicar si tienen el módulo Bluetooth integrado o no. Además, en la misma sección encontramos televisores de los cuales interesa saber, además del nombre, precio y stock, qué tecnología utilizan (ultraHd – 4K - FullHd) y la resolución en pixeles.  
Por otro lado, los cargadores portátiles que son de la sección cargadores almacenarán también la cantidad de cargas que pueden hacer sin necesidad de recargarlos.  
La tienda administra todos estos productos por lo que deberán crear los métodos necesarios que permitan agregar nuevos productos, modificarlos y eliminarlos. La tienda quiere conocer cuál es su producto con mayor stock y cual el de menor.

</details>

<details markdown="block">
<summary><strong>Unidad 5 - Modificadores</strong></summary>
  
### 1. Ejercicios anteriores
Hacer las modificaciones necesarias en cada una de las clases y método ya resueltas durante el año para que sean abstractas o estáticos si es necesario. 

### 2. Recetas
En una plataforma de recetas culinarias se definirán distintos platos que se podrán realizan indicando nombre del plato, nivel de dificultad (Fácil, medio o avanzado) y una lista de pasos para realizarlo.

Si lo que se quiere cargar es una receta de un plato principal, entonces habrá que agregar información sobre el tiempo de cocción y el número de comensales. Si es un postre, la temperatura del horno en el que se prepara y si es apto diabéticos o no. Para las entradas, agregar si es fría o caliente.

Es importante que sin importar de qué tipo de plato estamos hablando, en cualquier caso, se pueden mostrar las instrucciones en las que se detallan el paso a paso de la preparación. 

Para los platos principales habrá que mostrar: “Esta receta tarda en cocinarse + _tiempo de cocción_ y los pasos son: _lista pasos_”. Para los postres se muestra la lista de pasos, pero por cada paso recordar mantener la cocina limpia y el horno al mínimo. Para las entradas, si son frías recordar una vez que se termina de mostrar la lista de pasos que guarde la preparación en la heladera. En cambio, si es caliente, antes de mostrarle la lista de pasos recordarle que prenda el horno. 

Por último, nuestra plataforma deberá:  
- Permitir agregar, eliminar y modificar recetas.  
- Buscar recetas según dificultad. 
- Filtrar recetas por tipo (_Desafío_: Usarlo usando un único if) 
- Cantidad total de recetas cargadas. 
- Dar la receta con mayor cantidad de pasos.

### 3. Drones

Se quiere coordinar una flota de drones dedicada a entregas y tareas de vigilancia. Para eso tendremos drones que tienen un nombre de modelo, fecha de adquisición, nivel de carga y un contador que refleja cuántos drones operativos hay. Además, este número servirá como id de cada drone para rastrearlo si su estado es _en vuelo_ o _en operativo_. En cambio, si el estado es _inactivo_ o _mantenimiento_ no se podrán rastrear (tener en cuenta que los únicos estados del drone van a ser estos, no hay más) 
Todos los drones podrán recargar la batería: donde se asume que cada vez que se recarga se aumenta un 10%. Si la batería estaba por debajo del 20% cuando se quiere recargar, entonces va a 100%. 

Por último, los drones también tienen en común que podrán ejecutar misiones y comunicar al sistema si pueden realizarla con éxito o no. La misión se ejecuta dependiendo si son drones de carga o de vigilancia y en ambos casos se indica la latitud y longitud a la cual se tienen que dirigir. Todos parten desde el Poli (Latitud: -34.573195, Longitud: -58.504111)

Lo que hacen los drones de carga es guardar el peso de la carga que llevan y, al ejecutar una misión, en caso de que esté a 30 km o menos quiere decir que va a ser 3 viajes de ida y vuelta que le repercute en un 50% de batería. Si tiene la capacidad para hacerlo, entonces la misión será exitosa, sino no.

Para los drones de vigilancia tienen guardados la cantidad de memoria que tiene su sd. Entonces, deberán viajar hasta el destino y cada 2 km guardar una foto de la zona en la sd que ocupa 12 Mb. Se debe chequear antes de empezar la misión si tiene almacenamiento para realizarlo o no. 

_Sugerencia_: Utilizar el algoritmo de abajo que permite calcular la distancia en km en linea recta de un punto a otro 

```java
// Convertir a radianes 
double lat1Rad = Math.toRadians(latitudOrigen); 
double lon1Rad = Math.toRadians(longitudOrigen); 
double lat2Rad = Math.toRadians(latitudDestino); 
double lon2Rad = Math.toRadians(longitudDestino)); 
 
// Fórmula de Haversine 
double dLat = lat2Rad - lat1Rad; 
double dLon = lon2Rad - lon1Rad; 
double a = Math.sin(dLat / 2) * Math.sin(dLat / 2) + 
 Math.cos(lat1Rad) * Math.cos(lat2Rad) * Math.sin(dLon / 2) * Math.sin(dLon / 2); 
double c = 2 * Math.atan2(Math.sqrt(a), Math.sqrt(1 - a)); 
double radioTierraKm = 6371; 
return radioTierraKm * c; 
```

### 4. Gestión de mascotas
#### a)
Vamos a manejar una aplicación de mascotas. Estas pueden ser: perros, gatos, pájaros. 

Todas las mascotas tienen un nombre y un dueño (el nombre de la mascota debe ser único). Cada una tiene un saludo en particular:  
- Para los perros el saludo es “guau”  
- Para los gatos el saludo es “miau”  
- Para los pajaritos el saludo es “pio

Los pajaritos tienen una característica adicional, pueden ser o no cantores. Si son cantores hay que especificar cuál es su canto (diferente de “pio”).  

Se debe poder realizar un alta de mascotas donde se indique el nombre, dueño y tipo. También se deben poder eliminar mascotas y modificar mascotas.  

Dentro del menú de la aplicación debe existir la opción “Saludar”, la misma solicita el nombre al usuario y el nombre de la mascota. El programa debe responder:  

- Si el usuario es el dueño de la mascota: se saluda con el saludo de la mascota (por ejemplo: guau) 

- Si el usuario no es el dueño de la mascota: se saluda con el saludo de la mascota en mayúsculas y con un signo de exclamación (por ejemplo: GUAU!)

En el caso de los pajaritos la situación cambia, si el usuario no es el dueño no debe 	responder nada

#### b)
Se agregan peces como mascotas con 10 vidas iniciales. Los peces no tienen saludo, pero cada vez que los saluda el dueño pierden una vida, de lo contrario, si los saluda un NO dueño mueren.  

Para sumar vidas deben alimentarse mediante el método alimentar. Cada vez que se llama a dicho método se suma una vida. Si el pez se queda sin vida se debe eliminar automáticamente del listado de mascotas.  

#### c)
Para los perros, gatos y pajaritos también existe un método alimentar. Ese método suma alegría a la mascota. 

Por cada punto de alegría que tenga la mascota el saludo se prolonga. Por ejemplo, para un gato que tiene 3 puntos de alegría el saludo es “miau miau miau”.  

En los casos donde la alegría es mayor a 1 al saludar se resta un punto de alegría. Por ejemplo: 

> Un gato tiene 3 puntos de alegría:
>
> 1. Saluda una vez con “miau miau miau” y se le resta 1 a su alegría quedando en 2.  
> 2. Saluda nuevamente, esta vez con “miau miau” y se le resta 1 a su alegría quedando en 1.  
> 3. Saluda nuevamente, esta vez con “miau” pero como su alegría ya estaba en 1 no se modifica.  


Cada tipo de mascota debe tener un método el cual devuelve qué tipo de mascota es (Perro, Gato, Pajarito o Pez) 

### 5. Sistema de bebidas

Realizar un sistema que controle el consumo de bebidas de personas. Cada persona debe tener un nombre, apellido y DNI (el DNI debe ser único).

Las bebebidas tienen un nombre y un coeficiente de positividad y uno de negatividad. Existen 3 clases de bebidas:

- `Bebidas neutras`: en estas bebidas los coeficientes se establecen manualmente. 

- `Bebidas azucaradas`: en estas bebidas se establece un atributo llamado “cantidad de azúcar”, el coeficiente de positividad es siempre 1 y el de negatividad se calcula multiplicando la cantidad de azúcar por 10. 

- `Bebidas alcohólicas`: en estas bebidas se establece un atributo llamado “cantidad de alcohol”, el coeficiente de positividad es siempre cero y el de negatividad se calcula multiplicando la cantidad de alcohol por 20. 

Cada persona tiene una lista de bebidas que consumió indicando bebida y cantidad. Se debe poder calcular el coeficiente de hidratación resultante de cada persona. Por ejemplo:  

> Agua (coef. de negatividad = 0, coef. de positividad = 20)  
> ​Coca (cantidad de azúcar = 5)  
>  
> ​Si Juan tomó 3 aguas y 2 cocas:  
>  
> ​  Coeficiente resultante para 3 aguas = 3 x (20 - 0) = 60  
> ​  Coeficiente resultante para 2 cocas = 2 x [1 - (5 x 10)] = -98  
> ​  Coeficiente resultante total = 60 + (-98) = -38

Adicionalmente se debe poder calcular la persona con mejor y con peor coeficiente de hidratación y un método para que el usuario elija que bebida consumir y la cantidad.
</details>

<details markdown="block">
<summary><strong> Ejercicio repaso evaluación unidades 3, 4 y 5</strong></summary>
  
### 1. Gestión de tickets:

Tenemos un sistema que se ocupa de revisar la VTV de los autos que circulan por la ciudad. Se compone de Software y dispositivos como cámaras, radares y camiones. Cuando algo no funciona como debería, o un usuario no entiende una funcionalidad, o se quieren agregar cosas nuevas se pueden emitir Tickets. Estos le informan a la empresa desarrolladora qué está pasando con su sistema. 

Vamos a modelar la gestión de tickets de soporte técnico para este sistema. Todos los tickets tienen un cliente asignado, una descripción, una fecha y hora de creación, fecha y hora de finalización, una lista de comentarios donde los desarrolladores van a ir registrando anotaciones y estado del ticket: abierto, en progreso, resuelto, cerrado, cancelado. 

Es importante que los tickets puedan cambiar su estado, que se puedan agregar comentarios por parte del desarrollador y que se puedan resolver. Tener en cuenta que al cambiar de estado o, si se resuelve el ticket, hacer todas las modificaciones necesarias 

Los tickets pueden ser de hardware o de software. Para los de hardware vamos a guardar dispositivo y la forma de resolverlo es corroborando si hay repuestos disponibles para ese dispositivo. Si hay repuestos y el ticket estaba en progreso, cambiarlo a resuelto y retornar true, sino retornar false. 

Los tickets de software guardan el software sobre el que se está emitiendo el ticket y estos tienen una cantidad máxima de intentos de resolución que es igual para todos y es de 3 intentos. Para poder resolverlo, si el software tiene un parche aplicable y todavía restan intentos, entonces si estaba en progreso pasa a resuelto y retorna true. Si alguna de las dos condicionas falla, retorna false.  

Como parte de la gestión, tendremos una lista con los tickets de software y de hardware y los desarrolladores. Se querrá conocer: 

- Cantidad de tickets en un determinado estado. 
- Cantidad de tickets totales. 
- Ticket más antiguo que aún no ha sido agarrado por ningún desarrollador (es decir, el estado es abierto) 
- Desarrollador que más tickets resuelve. 
- Tickets asignados a un desarrollador determinado. 
- Desarrollador más antiguo en el sistema. 
- Dado un ticket determinado, conocer el o los desarrolladores asignados a resolverlo. 
- El tiempo promedio de resolución de los tickets en general. Para hacerlo calcular la diferencia entre fecha de resolución y fecha de creación y luego el promedio (Sugerencia: utilizar clase Duration)  

Resolver el sistema que responda de manera correcta a todas las funcionalidades mediante programación orientado a objetos. Incluir main. 

</details>

<details markdown="block">
<summary><strong> Unidad 6 - HashMaps y HashSets </strong></summary>
  
### 1. Vacunatorio

Se va a realizar una campaña nacional de vacunación y nos piden un sistema para registrar los ciudadanos ya vacunados. 

De cada ciudadano tenemos dni, nombre y apellido, provincia de residencia, domicilio y mail de contacto. A su vez, las vacunas tienen una fecha de fabricación, fecha de aplicación, numero de lote, numero de fabricacion y nombre comercial.

Se solicita poder tener en nuestro sistema lo necesario para que nos facilite:
- Registrar una vacuna aplicada a un ciudadano.
- Consultar el historial de vacunas de un ciudadano por dni.
- Obtener cuantas personas fueron vacunadas por Provincia
- Saber qué ciudadanos cumplen con tener una determinada cantidad de vacunas pasada por parametro.
- Conocer dado una vacuna determinada qué ciudadanos ya se la dieron.

### 2. Pago de empleados

La empresa "Creativos sin límites" desea gestionar el pago de sus empleados que son todos diseñadores. Estos tienen una comisión sobre los proyectos que realizan de acuerdo al tipo de diseñador según la siguiente tabla:

| Tipo de diseñador | Comisión | 
|---|---|
| UX | 8% | 
| UI | 7% | 
| IT | 12% | 

Un diseñador no puede realizar un mismo proyecto dos veces. Entonces, estos almacenan una lista de los proyectos junto a cuánto ganaron por hacer cada uno. Así, un diseñador debe poder:
- Conocer su sueldo. Para eso deberán adicionarle a la suma de lo que recaudó por todos los proyectos la comisión de acuerdo al tipo de diseñador que sea.
- Saber cantidad de proyectos realizados hasta el momento.
- Dado un proyecto determinado conocer cuánto gano sin comisión.
- Mostrar el detalle del sueldo discriminado para todos los proyectos que hizo. Es decir, por cada proyecto mostrar el nombre, cuánto gano y cuánto representa la comisión


### 3. Control altura y peso

Realizar un sistema que controle la altura y peso de una persona a través del tiempo. La persona debe tener un nombre, apellido y fecha de nacimiento. 

Cada persona cuando se pesa y mide debe registrar su peso y altura justo con la fecha. 

La persona debe tener una forma de conocer:  

- Su peso y altura en una fecha en particular.  

- El promedio de peso y de altura en un año.   

- El porcentaje de crecimiento de una fecha a otra.

### 4. Control calorías

Realizar un sistema que controle las calorías consumidas por personas dentro de una familia. Las personas se almacenarán en una entidad denominada familia, es decir, una familia va a tener muchas personas. 

Existirán platos los cuales tendrán nombre, ingredientes y cantidad de calorías que poseen.  

De las personas se desea conocer el nombre y fecha de nacimiento. Cada vez que una come un plato se debe guardar ese dato para luego saber:   

- Cantidad de calorías consumidas en total por la persona. 

- Promedio de calorías por familia. 

- Persona que consumió más calorías en la familia. 

- Persona que consumió menos calorías en la familia. 

### 5. Sistema de población

Realizar un abm de lugares. Los lugares pueden ser de tipo: **Barrio**, **Ciudad**, **Provincia o Estado**, **País**, **Continente**.

Todos los tipos de lugares tienen un nombre, código y una lista de coordenadas (latitud y longitud) que unidas representan el contorno del lugar

Las reglas de composición son:

- Una **ciudad** está compuesta por barrios.
- Una **provincia o estado** está compuesta por ciudades.
- Un **país** está compuesto por provincias o estados.
- Un **continente** está compuesto por países.

Para el caso de los barrios tendrán un atributo llamado `población`, el mismo indica la cantidad de habitantes del barrio. En los otros casos este atributo no existe, pero se desea calcular la población de forma automática.  

Tener en cuenta que en nuestro mundo se guardan una lista de Continentes. A realizar: 

- ABM (Alta, Baja y Modificación) de lugares
- Consulta de población de lugares por código de lugar
- Pantalla de información con:
  - País con más población
  - País con menos población
  - Continente con más población
  - Continente con menos población

</details>

<details markdown="block">
<summary><strong>Ejercicios repaso evaluación unidad 6</strong></summary>

### 1. Consumo de electricidad de viviendas
Realizar un sistema que administre el consumo de electricidad de viviendas. 

Cada vivienda tendrá una dirección, un código postal y un dueño asignado. El dueño deberá tener asociado un nombre, un apellido y un DNI. Si la vivienda es una casa, se guardarán los metros cubiertos por un lado y los descubiertos por otro. En cambio, si es un departamento se guarda la cantidad de ambientes.  

Una vez por mes se deberá cargar cuál fue el consumo de electricidad de cada vivienda. Al cargar el consumo se debe almacenar el mes (de enero a diciembre) y los KWh consumidos en ese periodo, comprobando que el mes no esté ya cargado para esa vivienda.  

Además de permitir cargar el consumo, se debe generar el método correspondiente para poder calcular lo que debe pagar cada vivienda por su consumo. Para dicho cálculo se utilizan dos valores:  
- Para casas: $100 el KWh
- Para departamentos: $50 el KWh  

_Ejemplo: si una casa consumió en un mes 20KWh debe pagar $2000._

Por otro lado, si el consumo del mes se redujo un 10% respecto del consumo del mismo mes del año anterior se debe aplicar un descuento del 5% al número final. 
Realizar las clases correspondientes con sus métodos asociados y un programa de prueba que demuestre el buen funcionamiento del sistema y cálculos ejemplo de lo que deben pagar las viviendas.  

### 2. Estructura ONG

Todas las personas que participan dentro de una ONG se registran indicando nombre, apellido, fecha de nacimiento, dirección, código postal y si desean registrarse para contribuir con una mensualidad o no. 

Además, dentro de la organización hay distintos roles: Voluntarios miembro, voluntarios externos, administradores y profesores (titulares e interinos). Cabe destacar que los voluntarios no reciben un sueldo por lo que hacen mientras que los administradores y profesores sí. 

Los voluntarios miembros tienen un puntaje que se va modificando cada vez que realizan una acción solidaria. De los voluntarios externos habrá que guardar la institución en la que trabajan indicando el nombre y dirección de esta.  

Dentro de los que reciben un sueldo, habrá que guardar en qué banco se deposita el sueldo (Macro, Santander, BBVA y HSBC), la fecha de cobro y la fecha de alta en la empresa.  

Si es un personal administrativo, es importante saber qué computadora utiliza (código alfanumérico) así como su nombre de usuario y la contraseña (verificar que tenga mínimo 8 caracteres, una mayúscula y algún carácter especial). Estos datos, en caso de que sea profesor, no importan. Sí será relevante almacenar el nombre de la materia que dictan y la cantidad de horas que trabajan. Todos los profesores interinos dan más de una materia por lo que habrá que guardar la información de todas las que enseña junto con la cantidad de horas.  

Otra cosa que diferencian a las personas que participan de las ONG son las zonas barriales que visitan ya que se distribuyen en toda la capital de Buenos Aires. Dados los 48 barrios porteños, todos los voluntarios miembros se desarrollarán en: _Montserrat, Nueva Pompeya, Nuñez, Belgrano y Constitución_, todos los voluntarios externos lo harán en: _Coghlan, Palermo, Barracas, Parque Patricios, Retiro y Saavedra_, todos los profesores en: _Puerto Madero, San Cristóbal, Palermo, Monte Castro, Versalles, Villa Santa Rita y Colegiales_ y, por último, todos los administrativos estarán en: _Flores, Floresta, Agronomía, Colegiales y Parque Chas_ 

Además de confeccionar la estructura correspondiente, se solicitan las siguientes funcionalidades:

- Todos realizan una acción solidaria acorde al rol en el que están. La acción solidaria para los voluntarios consiste en mostrar un cartel que diga: “Ofrezco mi ayuda para lo que necesiten” además de sumarle un punto a su puntaje (si es voluntario miembro). Los administrativos deberán mostrar su usuario de pc junto al nombre y los profesores la o las materias que dictan en la ONG (dependiendo si es interino o no).  

- Tanto de los asalariados como de los voluntarios importa saber si son mayores de edad o no.  

- De los integrantes de la organización se mostrará el nombre de los incorporados hace menos de 2 meses.  

- Mostrar de cada banco la cantidad de trabajadores que cobran el sueldo por ese medio. 

</details>

<details markdown="block">
<summary><strong>Unidad 7 - Manejo de excepciones</strong></summary>

### 1. Ejecutar el siguiente fragmento de código:  

```java
public class Main {  
    public static void Main(String[] args) {  
        String nombre = null;  
        System.out.println("El largo del nombre es:" + nombre.length);  
    }  
}
```
Resolver la excepción de cuatro formas diferentes. Siempre al final del programa 	habrá que mostrar el nombre de ustedes a modo de firma:  
- Bloque try/catch.  
- Throw. 
- Throws. 
- Clase personalizada.

### 2. Sistemas de alarmas (ejercicio 5, unidad 3)

Dado el ejercicio de sistema de alarmas que tiene un edificio (ejercicio 5, unidad 3), habrá que permitirle al usuario que pueda elegir de cuál de todos los dispositivos quiere obtener más información.  

Para esto habrá que pedirle al usuario que ingrese un número desde el 0 hasta la cantidad de alarmas que estén registradas. Acorde al número que elija es el dispositivo que se mostrará. 

Deberán tener en cuenta en la implementación que no se corte la ejecución del programa si el usuario no ingresa un número entero o ingresa un número mayor a la cantidad de dispositivos que hay instalados en el edificio. 

### 3. Sistema componentes de pc (ejercicio 4, unidad 3)

Agregarle al sistema de compras de componentes de computadora (ejercicio 4, unidad 3) las excepciones necesarias para que el usuario sepa si no hay stock de los componentes que eligió y lanzar una excepción en caso de que al hacer la compra falte uno de los componentes principales (una CPU, un dispositivo de entrada y uno de salida). 

### 4. Biblioteca virtual

Vamos a hacer un programa que me permita gestionar una biblioteca virtual con libros electrónicos, autores, usuarios y préstamos. 

Los géneros de los libros pueden ser: ficción, no ficción, aventura, ciencia ficción, saga y romance. Los libros van a ser escritos por un autor del cual interesa conocer el nombre, la fecha de nacimiento, el dni y su bibliografía (todos los libros que escribió). 

De cada libro electrónico se guardará el título, el autor, el género, el nombre del archivo pdf y la cantidad de descargas disponibles que tiene: 145 (es igual para todos los libros). 

Los usuarios de la plataforma se registran ingresando nombre, fecha de nacimiento, DNI, mail y el tipo de membresía que tiene. Si es bronce podrá tener hasta 5 libros prestados, Plata como mucho 15 libros y si es oro 50 préstamos activos. 

El sistema debe gestionar los préstamos y devoluciones de libros electrónicos. Si un usuario intenta tomar prestado un libro que ya ha alcanzado el límite, se debe lanzar una excepción personalizada (LimiteDePrestamosAlcanzadoException). Así como hay que lanzar la excepción (‘MembresiaException’) si el usuario ya alcanzó su cupo de libros que puede tomar prestados simultáneamente. 

Además, hacer los métodos necesarios para poder agregar, borrar o modificar nuevos libros. En la clase 'Main' crea instancias de autores, libros electrónicos, usuarios y bibliotecarios para poder realizar operaciones de préstamo y devolución, y maneja las excepciones adecuadamente. 

### 5. Sistema de bebidas (ejercicio 5, unidad 5)

Añadir al ejercicio 3 de la unidad 6 el manejo de excepciones para corroborar que: 
- Al añadir personas al sistema ya no exista ese dni. 
- Encuentre la bebida que quiere consumir y tenga esa cantidad que solicita. 
- Existen personas registradas para determinar el de mejor y peor coeficiente de hidratación. 
</details>

<details markdown="block">
<summary><strong>Unidad 8 - Interfaces polimórficas</strong></summary>

### 1. Elecciones en Octubre:  

En época de elecciones, tenemos un sistema que administra la organización de los partidos políticos del país. Estos se manejan haciendo campaña de 3 formas como son las palomas mensajeras, los teléfonos móviles y los trabajadores.  

Sabemos que las palomas mensajeras son un tipo específico de ave donde, además de guardar el color, nombre y especie que es común a todas las aves, se guardará también una variable que indique si ya aprendió el mapa para volar sola o no.  

Por otro lado, los teléfonos móviles pertenecen al grupo de dispositivos por lo que, si bien es común para todo dispositivo el número de serie, fabricante y modelo, el teléfono móvil deberá guardar en particular a qué compañía telefónica pertenece {Claro, Personal, Movistar o Tuenti} y el número celular.  

En el caso de los trabajadores habrá que conocer no sólo el nombre, apellido, dni, fecha de nacimiento sino también el número de cuil, el sueldo y la dirección de residencia.  

Las personas, los teléfonos móviles y las palomas mensajeras para cumplir con lo que les pide su partido político envían mensajes en apoyo de los dirigentes del partido al cual militan. Cada partido tiene un nombre, un dirección donde se encuentra la oficina central, una cantidad de afiliados y una lista de los enviadores de mensajes.  

Se deberá hacer un método para que se pueda agregar un mensajero a dicha lista y otro titulado: hacer campaña. Este consiste en recorrer todos los mensajeros afiliados y por cada uno enviar un mensaje que diga: “Vote por el partido para un mejor futuro”. Este mensaje, si es dado por una paloma mensajera deberá ser precedido por el siguiente lema: “Lanzando un papelito que dice:”. Eso sí, hay que tener en cuenta que el mensaje sólo lo puede enviar si ya aprendió a volar. Si el mensaje se transmitE por un teléfono móvil al mensaje oficial del partido le antecederá: “Conectando con la antena más cercana” siempre y cuando el teléfono esté prendido y tenga crédito disponible. Por último, si un trabajador transmite el mensaje, primero habrá que verificar si está en su horario laboral y luego deberá decir antes del mensaje común: “Yo, nombreTrabajador te invito a que…” 

### 2. Campeonato de arco y flecha:

En los nuevos bares de CABA se ha instalado la moda de jugar al arco y flecha. Para esto nos solicitaron un sistema en el que se pueda manejar el sistema de puntos y de beneficios que obtiene el cliente que participa de los tiros de arco y flecha. 

En nuestro sistema tendremos una lista de bares que implementan el arco y flecha, una lista de todos los tipos de diana y una lista de todos los beneficios que ofrece este juego. 

De cada bar se guardará una lista de las dianas que utiliza, la cantidad de clientes que juegan al arco y flecha, el dinero recaudado, una lista de todos los beneficios que decide implementar y una lista de sólo los beneficios acumulables. 

Para el caso de los beneficios interesa guardar el nombre del beneficio y quién fue el usuario creador (alcanza con guardar solo el nombre de la persona). Si es un beneficio de gaseosa, se almacenan también a una lista de las gaseosas. Si es un beneficio de comidas, se almacenan también una lista de las comidas. Si es un beneficio de tragos, se almacenan también a una lista de los tragos. 

La particularidad que tienen los beneficios es que no todos son acumulables. Únicamente son acumulables los beneficios de gaseosas y comidas. Esto quiere decir que sólo los beneficios de gaseosas y comidas tienen el método aplicarDescuentoExtra que para las gaseosas retorna $1000 y para las comidas $4500. 

Las Dianas se dividen en tres tipos: Circulares, rectangulares y cuadradas. Todas las dianas tendrán un nombre identificatorio, un nivel de dificultad y una lista que relaciona el puntaje en cada franja con el color (los colores pueden ser sólo rojo, verde, amarillo, blanco o negro). Tener en cuenta que los puntajes no se repiten en una misma diana.  Además de eso, a todas las dianas circulares se les agrega el valor del radio que es de 13cm, a las dianas rectangulares se les agrega el valor de la altura y la base y a las dianas cuadradas se pide guardar el valor del lado. 

Se solicita: 

- Poder calcular el área de cualquier tipo de diana. Si es circular el cálculo será 
_π × radio × radio_, si es el cálculo del área del rectángulo entonces _base × altura_ y si es un cuadrado: _lado × lado_. 

- Para cada bar se quiere saber cuántos beneficios de tragos tiene. Es decir, aquellos beneficios no acumulables. 

- Retornar la diana de nuestro sistema que tenga más cantidad de puntajes distintos.  

- Realizar un main donde se prueben todas las funcionalidades pedidas.

### 3. Tratamiento de modificación de sangre:

En la fundación endocrinológica están haciendo una investigación sobre un tratamiento para modificar la sangre de los pacientes. Tienen una dudosa hipótesis de que, si todos los jóvenes tienen sangre A+ y todos los niños tienen sangre AB entonces sería más fácil evitar la multiplicación de enfermedades. 

De cada paciente se guardó el nombre, apellido, fecha de nacimiento, el género y su tipo de sangre: A, B, AB y O. (tener en cuenta que cada tipo puede ser + o -). Luego, una vez recolectada esa información, se dividió a los pacientes en: Niños, Jóvenes, Adultos y Gerontes.  Según qué tipo de paciente es se guardará una información distinta y, la forma en la que se tratará también. En particular, solo tenemos información de cómo responden al tratamiento los jóvenes y niños, los Gerontes y Adultos aún no califican en este experimento, pero sí son parte del sistema. 

De los jóvenes se guardará para todos los de esta categoría la edad mínima y máxima para pertenecer que es de 20 a 30 años respectivamente y las actividades deportivas que hacen. Si la cantidad de actividades que hacen es impar y les quedan 2 años o menos en esta categoría se les dirá: “Lamentamos comunicarte que tu sangre aún no va a poder ser modificada” y sino: “Será un tratamiento costoso, pero lo vamos a lograr”. 

De los niños nos interesa saber el nivel de tolerancia a los medicamentos (1 menos tolerante y 10 más tolerante) y si tiene más de 3 años. Al solicitar tratamiento, si tiene más de tres años se mostrará un mensaje que diga: “Tu tratamiento tardará esta cantidad de días: ... (nivel de tolerancia * 2)”. Sino le mostramos: “Aún es chico para probar el tratamiento” 

Además, el costo del tratamiento varía según el tipo de paciente que sean (Jóven o Niño). Para los niños hay que multiplicar el nivel de tolerancia * $450.000. Por otro lado, para los jóvenes con fecha de nacimiento en año impar el costo es el número de mes * $760.000, sino es el número de día * $145.400 

En nuestro sistema tendremos guardados por un lado los pacientes que califican con el tratamiento (por ahora solo los jóvenes y niños) junto a los días de tratamiento que llevan y en el otro todos los pacientes que fueron (niños, jóvenes, adultos y gerontes).  

Se solicita realizar un método que la fundación ejecutará todos los días y consiste en recorrer los pacientes en tratamiento y si pueden solicitar tratamiento se le suma uno a la cantidad de días que llevan en tratamiento. Luego, queremos otro método que diga la cantidad de pacientes que no aplican al tratamiento, es decir, la cantidad de Gerontes y Adultos que fueron a la fundación. 

__Aplicar las clases, atributos, métodos e interfaces necesarias para poder cumplir con las funcionalidades del sistema y realizar un main donde se cumple con lo solicitado__

</details>

---

# Ejercicios repaso evaluación unidades 7 y 8

### 1. Masterchef edición labo

En el nuevo programa de cocina los participantes cocinan distintos platos. Estos se anotan indicando nombre, apellido, fecha de nacimiento, localidad y color de equipo al que pertenece: rojo, verde o azul.

Dentro de la competencia los participantes se dividen en tipos: 
- Principiantes
- Intermedios
- Expertos. 

Para los participantes principiantes se guarda una lista de los ingredientes prohibidos que no puede usar en las recetas, los participantes intermedios cuentan con un stock propio de ingrediente y la cantidad correspondiente y los expertos no tienen ninguna restricción de alimentos ni stock, sino que tienen un tiempo límite para la preparación de sus recetas que es para todos los expertos igual: 80 min.

Todos tendrán un método que les prepare el lugar de trabajo y según el tipo de participante es cómo responden a esto:
- Los principiantes imprimen un mensaje que dice: “Ya guarde todos los elementos prohibidos y no voy a usar: ….. (muestra todos los nombres de los ingredientes prohibidos)”
- Los intermedios muestran un mensaje que dice: “Mi stock a utilizar es de ….(muestran nombre solo de los ingredientes que tengan una cantidad >1”
- Los expertos muestran un mensaje que dice: “Perdi 5 minutos preparando la mesa por lo que mi tiempo restante es: ….(muestra el tiempo restante actual para cocinar)”

Luego, sabemos que los principiantes solo pueden cocinar y servir platos de entrada, los intermedios solo cocinar y servir platos principales, y los expertos podrán cocinar y servir tanto platos de entrada como platos principales. Estas dos funcionalidades se implementan distinto según el nivel del participante. Tener en cuenta que si se quiere cocinar un plato que no tiene los ingredientes necesarios o no alcanza el tiempo de preparado o tiene algún elemento prohibido lanzar la excepción correspondiente.

El main donde se prueban las funcionalidades se debe llamar: MasterChefApp (sin excepción). Importante que antes de correr la clase corrector deberán correr su propio main para que se genere la carpeta out.

**Descargar el corrector a incluir en el proyecto:**  
[CorrectorMasterChef.java](https://github.com/ProfesLabo5to/ResolucionEjercicios/blob/main/CorrectorMasterChef.java)

### 2.Préstamos virtuales

Se busca desarrollar un sistema para gestionar una biblioteca virtual que incluya el control de préstamos de diferentes tipos de contenidos y los usuarios que lo utilizan.

Los usuarios guardarán nombre, apellido, fecha de nacimiento, crédito ganado, mail y lista de todas las publicaciones que haya leído y otra lista donde solo tenga la lista de las publicaciones que pidió a préstamo y las veces que lo hizo.

Tener en cuenta que en nuestro sistema cuando viene un usuario a devolver un préstamo es que se verifica que ese préstamo esté en fecha y al validarse correctamente se le suma uno en la lista de prestamos que hizo y la cantidad de veces. Si esto no sucede, enviar una excepción: “Prestamo devuelto fuera de fecha” y se calcula la multa. Esto devuelve un valor que hay que restarle al crédito del usuario y depende el tipo de publicación.

Cada publicación que se encuentra tiene información básica, como título, autor, año de publicación y stock. Los tipos de publicaciones pueden ser libros (se agrega si tiene saga o no), revistas (se agrega nombre de la distribuidora) y audiolibros (se agrega duración del y peso del archivo)

Para gestionar los préstamos, se almacena información sobre el artículo, el número de socio, la fecha de préstamo y la fecha de devolución estimada. Por ahora solo se pueden dar a préstamos los libros y revistas. La multa de los libros es de $7500 pesos y la de las revistas $3500

De esta forma, dar a préstamo un libro implica poner que la fecha de devolución es 15 días más tarde y mostrarle al usuario el título de lo que se está llevando junto a cuando lo tiene que devolver.  Para las revistas, si el año de publicación es menor a 2020 entonces la fecha de devolución tiene que ser 10 días más tarde y sino la fecha de devolución son 3 días más tarde. 

Luego de hacer la programación necesaria para poder dar a préstamo las publicaciones que tienen esa posibilidad, en el sistema bibliotecario se quieren almacenar tres cosas: Las publicaciones totales que tienen en el sitio, por un lado, las publicaciones que pueden ser dadas a préstamos (en este caso solo los libros y revistas, pero podría verse modificado) por otro y todos los prestamos realizados.  
 
1.	Realizar un motor de búsqueda que dado el nombre me busca entre todas las publicaciones si existe. En caso afirmativo devolver el título, autor y año de publicación. Si además es un contenido que puede ser prestado, agregarle una leyenda que diga: “Si quiere tómelo prestado”. Por otro lado, si no existe el nombre lanzar una excepción que diga: “No tenemos el libro”.
2.	Poder antes de realizar un préstamo verificar si está disponible el artículo o no. Es decir, que sea un objeto con la posibilidad de dar a préstamo y que tenga el stock suficiente. Lanzar las excepciones correspondientes si algo falla (“No se puede dar a prestamo” o “No hay stock suficiente”) o sino mostrar un mensaje de éxito (“Estpa disponible para ser prestado”).
3.	Realizar el método agregarPrestamo. Sabemos que recibe un objeto que puede ser dado a préstamo (por ahora, libro o revista nada más). Lo que va a hacer agregar es llamar al método darPrestamo del objeto que se quiere dar a préstamo para que se actualice la fecha de devolución del préstamo según lo que el método devuelve. Entonces, se crea el préstamo con esa información y se agrega a la lista de préstamo realizado. Mostrar un mensaje de que se agregó el préstamo correctamente.
4.	En caso de que un usuario venga  a solicitar una extensión del préstamo, la primer condición para que esto suceda es que el crédito del usuario no sea negativo y tenga como mucho un prestamo activo ademas de ese. Luego, para el caso de los libros se podrá extender si hay mas de 5 en stock y para el caso de la revista si el nombre de la distribuidora tiene mas de 10 caracteres. Lanzar la excepción correspondiente si algo falla (“No es posible extender el préstamo”) o sino un mensaje de éxito (“Prestamo extendido”)

El main donde se prueben las funcionalidades se debe llamar: BibliotecaApp (sin excepción). Importante que antes de correr la clase corrector deberán correr su propio main para que se genere la carpeta out

**Descargar el corrector a incluir en el proyecto:**  
[CorrectorPrestamos.java](https://github.com/ProfesLabo5to/ResolucionEjercicios/blob/main/CorrectorPrestamos.java)

