

  
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

---


## Unidad 5 - Modificadores

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

<!-- línea en blanco antes y después de cada bloque <details> -->
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

---


