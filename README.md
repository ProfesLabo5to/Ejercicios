

# Ejercicios
Acá se subirán todos los ejercicios correspondientes a las unidades del Laboratorio de Programación Orientado a Objetos 2025.

<!-- Dejar siempre UNA línea en blanco antes del <details> -->

<details>
<summary><strong>Unidad 0 - Introducción y repaso al laboratorio</strong></summary>
  
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

<!-- Y otra línea en blanco para separar del siguiente bloque -->

<details>
<summary><strong>Unidad 1 - Clases y objetos</strong></summary>
  
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
<details>
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

<details>
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

<details>
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

---

## Unidad 4 - Enums

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
