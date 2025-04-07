
# Ejercicios
Acá se subirán todos los ejercicios correspondientes a las unidades del Laboratorio de Programación Orientado a Objetos 2025.


## Unidad 0 - Introducción y repaso al laboratorio



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

---

## Unidad 1 - Clases y objetos

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

