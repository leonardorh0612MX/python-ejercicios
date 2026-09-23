# Ejercicios de Python — de menor a mayor dificultad

## Cómo usar este archivo

1. Crea un archivo por ejercicio dentro de `ejercicios/`, con el nombre que se sugiere.
2. Resuélvelo sin mirar soluciones. Si te trabas 20 minutos, pasa al siguiente y vuelve después.
3. Cuando termines uno (o varios), me lo pasas y te lo reviso: corrección, estilo, y cómo lo haría un pythonista.
4. No saltes niveles completos. Sí puedes saltar algún ejercicio suelto que te resulte trivial.

**Regla de oro:** todo ejercicio debe poder ejecutarse con `python ejercicios/01_hola.py` y hacer algo visible.

---

## Nivel 0 — Primeros pasos
*Variables, tipos, `print`, `input`, operadores.*

### 01. Hola mundo con nombre — `01_hola.py`
Pide el nombre al usuario y saluda: `¡Hola, Leo! Bienvenido a Python.`

### 02. Calculadora de dos números — `02_calculadora.py`
Pide dos números y muestra suma, resta, multiplicación, división, división entera, módulo y potencia.

### 03. Conversor de temperatura — `03_temperatura.py`
Pide grados Celsius y muestra Fahrenheit y Kelvin, redondeado a 2 decimales.
`25 °C  ->  77.00 °F  |  298.15 K`

### 04. Área y perímetro — `04_circulo.py`
Pide el radio de un círculo y muestra área y perímetro usando `math.pi`.

### 05. Segundos a tiempo — `05_segundos.py`
Pide una cantidad de segundos y muéstrala como `HH:MM:SS`.
`3671  ->  01:01:11`

### 06. Intercambio de variables — `06_intercambio.py`
Pide dos valores, muéstralos, intercámbialos sin usar una variable temporal, y vuelve a mostrarlos.

### 07. Índice de masa corporal — `07_imc.py`
Pide peso (kg) y altura (m), calcula el IMC y muéstralo con 1 decimal.

### 08. Ticket de compra — `08_ticket.py`
Pide precio unitario, cantidad y porcentaje de IVA. Muestra subtotal, IVA y total alineados en columnas usando f-strings con formato (`f"{total:>10.2f}"`).

---

## Nivel 1 — Condicionales
*`if` / `elif` / `else`, operadores lógicos, comparaciones.*

### 09. Par o impar — `09_par_impar.py`
Pide un número entero y di si es par o impar.

### 10. Mayor de tres — `10_mayor_de_tres.py`
Pide tres números y muestra el mayor. **Sin usar `max()`.**

### 11. Clasificador de IMC — `11_imc_clasifica.py`
Reutiliza el ejercicio 07 y añade la categoría: bajo peso (<18.5), normal (18.5–24.9), sobrepeso (25–29.9), obesidad (≥30).

### 12. Año bisiesto — `12_bisiesto.py`
Pide un año y di si es bisiesto. Reglas: divisible entre 4, salvo que sea divisible entre 100, a menos que también lo sea entre 400.

### 13. Nota a letra — `13_nota.py`
Pide una nota de 0 a 100 y devuelve A/B/C/D/F. Valida que esté en rango; si no, avisa.

### 14. Piedra, papel o tijera — `14_ppt.py`
Una sola ronda: el usuario elige, la máquina elige al azar (`random.choice`), y dices quién gana.

### 15. Triángulo válido — `15_triangulo.py`
Pide tres lados. Di si forman un triángulo y, si lo forman, de qué tipo es: equilátero, isósceles o escaleno.

---

## Nivel 2 — Bucles
*`while`, `for`, `range`, `break`, `continue`, acumuladores.*

### 16. Cuenta regresiva — `16_cuenta_atras.py`
Pide un número N e imprime desde N hasta 1, y luego `¡Despegue!`.

### 17. Tabla de multiplicar — `17_tabla.py`
Pide un número y muestra su tabla del 1 al 10.

### 18. Suma y promedio — `18_promedio.py`
Pide números uno por uno hasta que el usuario escriba `fin`. Muestra cuántos ingresó, la suma y el promedio.

### 19. Factorial — `19_factorial.py`
Calcula el factorial de un número con un bucle. (La versión recursiva viene en el nivel 6.)

### 20. Fibonacci — `20_fibonacci.py`
Imprime los primeros N números de Fibonacci.

### 21. ¿Es primo? — `21_primo.py`
Di si un número es primo. Optimiza: basta probar divisores hasta `int(n**0.5) + 1`.

### 22. Adivina el número — `22_adivina.py`
La máquina piensa un número del 1 al 100. El usuario adivina; respondes "más alto"/"más bajo" y cuentas los intentos.

### 23. Pirámide de asteriscos — `23_piramide.py`
Pide una altura e imprime una pirámide centrada:
```
  *
 ***
*****
```

### 24. Invertir un número — `24_invertir_numero.py`
Invierte los dígitos de un entero **usando aritmética** (`% 10` y `// 10`), sin convertirlo a string.

### 25. Dígitos y suma — `25_suma_digitos.py`
Pide un número y muestra cuántos dígitos tiene y la suma de esos dígitos.

---

## Nivel 3 — Strings
*Indexación, slicing, métodos de `str`, f-strings.*

### 26. Contar vocales — `26_vocales.py`
Cuenta cuántas vocales tiene una frase (mayúsculas y acentos incluidos).

### 27. Palíndromo — `27_palindromo.py`
Di si una frase es palíndroma ignorando espacios, mayúsculas y signos de puntuación.
`"Anita lava la tina" -> True`

### 28. Contador de palabras — `28_contar_palabras.py`
Cuenta palabras de un texto y muestra la más larga.

### 29. Capitalizar títulos — `29_titulo.py`
Convierte `"el señor de los anillos"` en `"El Señor de los Anillos"` dejando en minúscula artículos y preposiciones (`de`, `la`, `los`, `el`, `y`, `en`).

### 30. Cifrado César — `30_cesar.py`
Cifra y descifra un texto desplazando letras N posiciones. Respeta mayúsculas y deja intactos los no-alfabéticos.

### 31. Validador de contraseña — `31_password.py`
Comprueba que una contraseña tenga ≥8 caracteres, una mayúscula, una minúscula, un dígito y un símbolo. Informa exactamente qué le falta.

### 32. Formateador de nombres — `32_nombres.py`
De `"  gARCÍA  , juan carlos "` produce `"Juan Carlos García"`. Limpia espacios sobrantes.

### 33. Anagramas — `33_anagramas.py`
Di si dos palabras son anagramas ignorando espacios y mayúsculas.

---

## Nivel 4 — Listas y tuplas
*Índices, slicing, métodos, ordenamiento, listas anidadas.*

### 34. Estadísticas de una lista — `34_estadisticas.py`
Dada una lista de números, calcula mínimo, máximo, suma, promedio y mediana. El mín/máx hazlos a mano con un bucle.

### 35. Sin duplicados — `35_sin_duplicados.py`
Elimina duplicados de una lista **conservando el orden original**.

### 36. Rotar lista — `36_rotar.py`
Rota una lista N posiciones a la derecha. `[1,2,3,4,5]` con N=2 -> `[4,5,1,2,3]`.

### 37. Intersección y diferencia — `37_conjuntos_listas.py`
Sin usar `set`, calcula los elementos comunes y los que están solo en la primera lista.

### 38. Burbuja — `38_burbuja.py`
Implementa el ordenamiento burbuja. Imprime el número de intercambios realizados.

### 39. Búsqueda binaria — `39_busqueda_binaria.py`
Busca un valor en una lista ordenada y devuelve su índice, o -1 si no está. Cuenta cuántas comparaciones hizo.

### 40. Matriz — `40_matriz.py`
Con una lista de listas 3×3: imprímela con formato, calcula la suma de cada fila, de cada columna y de la diagonal.

### 41. Agenda de contactos — `41_agenda.py`
Lista de tuplas `(nombre, teléfono)`. Menú en bucle: agregar, listar ordenado por nombre, buscar, eliminar, salir.

---

## Nivel 5 — Diccionarios y conjuntos
*`dict`, `set`, iteración, conteo, agrupación.*

### 42. Frecuencia de letras — `42_frecuencia.py`
Cuenta cuántas veces aparece cada letra de una frase y muestra el top 5 ordenado de mayor a menor.

### 43. Inventario — `43_inventario.py`
Diccionario `producto -> (cantidad, precio)`. Añadir, vender (validando stock), listar y mostrar el valor total del inventario.

### 44. Invertir diccionario — `44_invertir_dict.py`
Dado `{"a": 1, "b": 2, "c": 1}`, produce `{1: ["a", "c"], 2: ["b"]}`.

### 45. Agrupar por inicial — `45_agrupar.py`
Dada una lista de nombres, agrúpalos en un diccionario por su letra inicial.

### 46. Dos conjuntos — `46_sets.py`
Con dos listas de números, muestra unión, intersección, diferencia y diferencia simétrica usando `set`.

### 47. Traductor mini — `47_traductor.py`
Diccionario español→inglés. Traduce una frase palabra por palabra, dejando sin traducir las que no estén y marcándolas entre corchetes.

### 48. Votaciones — `48_votos.py`
Dada una lista de votos, cuenta cada candidato, declara al ganador y detecta empates.

---

## Nivel 6 — Funciones
*Parámetros, retorno, valores por defecto, `*args`/`**kwargs`, ámbito, recursión.*

### 49. Refactor a funciones — `49_refactor.py`
Toma los ejercicios 12 (bisiesto), 21 (primo) y 27 (palíndromo) y conviértelos en tres funciones puras con `return`. Pruébalas desde un bloque `if __name__ == "__main__":`.

### 50. Calculadora con funciones — `50_calc_funcs.py`
Una función por operación + un diccionario `{"+" : suma, ...}` que despache según el operador elegido.

### 51. Valores por defecto — `51_saludo.py`
`saludar(nombre, saludo="Hola", signos=True)` con distintas combinaciones de argumentos posicionales y por nombre.

### 52. `*args` y `**kwargs` — `52_args_kwargs.py`
`resumen(*numeros, **opciones)` que acepte cualquier cantidad de números y opciones como `redondeo=2` o `ordenar=True`.

### 53. Factorial y Fibonacci recursivos — `53_recursion.py`
Versión recursiva de ambos. Compara el tiempo de Fibonacci recursivo vs. iterativo para n=30 con `time.perf_counter()`.

### 54. Torres de Hanói — `54_hanoi.py`
Resuelve Hanói recursivamente e imprime cada movimiento. Cuenta el total.

### 55. Suma anidada — `55_suma_anidada.py`
Suma todos los números de una lista con listas anidadas a cualquier profundidad: `[1, [2, [3, [4]]], 5] -> 15`.

### 56. Validador reutilizable — `56_input_seguro.py`
`pedir_entero(mensaje, minimo=None, maximo=None)` que repita hasta recibir un entero válido en rango. Úsalo de aquí en adelante.

---

## Nivel 7 — Comprensiones y funciones de orden superior
*List/dict/set comprehensions, `lambda`, `map`, `filter`, `sorted(key=...)`, `enumerate`, `zip`.*

### 57. Comprensiones básicas — `57_comprensiones.py`
En un solo archivo: cuadrados del 1 al 20, solo los pares, los múltiplos de 3 que no lo sean de 5, y una lista de tuplas `(n, n²)`.

### 58. Reescribe con comprensiones — `58_reescribe.py`
Vuelve a resolver los ejercicios 26, 35 y 42 usando comprensiones. Compara la legibilidad con tu versión original.

### 59. Ordenar por clave — `59_ordenar.py`
Lista de diccionarios `{"nombre":..., "edad":..., "nota":...}`. Ordena por edad, por nota descendente, y por nota y desempata por nombre.

### 60. `zip` y `enumerate` — `60_zip_enumerate.py`
Con dos listas (nombres y notas) construye un diccionario, e imprime un listado numerado.

### 61. map / filter / reduce — `61_map_filter.py`
Aplica descuentos a una lista de precios, filtra los mayores a 100 y súmalos con `functools.reduce`. Luego reescríbelo sin `map`/`filter` y decide cuál prefieres.

### 62. Matriz transpuesta — `62_transpuesta.py`
Transpón una matriz con comprensión anidada, y luego con `zip(*matriz)`.

---

## Nivel 8 — Archivos y errores
*`open`, context managers, `csv`, `json`, `try/except/else/finally`, excepciones propias.*

### 63. Leer y escribir texto — `63_archivos.py`
Escribe 5 líneas en `datos.txt`, léelo y muestra el contenido numerado. Usa siempre `with`.

### 64. Estadísticas de un archivo — `64_stats_archivo.py`
Cuenta líneas, palabras y caracteres de un archivo de texto. Muestra las 10 palabras más frecuentes.

### 65. Manejo de errores — `65_errores.py`
Una función que divida dos números capturando `ZeroDivisionError` y `ValueError`, con `else` y `finally`. Muestra qué se ejecuta en cada caso.

### 66. Excepción propia — `66_excepcion_propia.py`
Define `SaldoInsuficienteError` y úsala en una función `retirar(saldo, monto)`.

### 67. CSV de notas — `67_csv_notas.py`
Lee un CSV de `alumno,materia,nota`, calcula el promedio por alumno y escribe un nuevo CSV con los resultados ordenados.

### 68. JSON persistente — `68_json_tareas.py`
Gestor de tareas que guarda en `tareas.json`: agregar, listar, marcar completada, eliminar. Los datos sobreviven al cerrar el programa.

---

## Nivel 9 — Programación orientada a objetos
*Clases, `__init__`, métodos, `@property`, herencia, dunder methods, `dataclass`.*

### 69. Clase Rectángulo — `69_rectangulo.py`
Atributos base y altura; métodos `area()` y `perimetro()`; `__str__` legible.

### 70. Cuenta bancaria — `70_cuenta.py`
`depositar`, `retirar` (usando la excepción del 66), historial de movimientos y `saldo` como `@property` de solo lectura.

### 71. Herencia de figuras — `71_figuras.py`
Clase base `Figura` con `area()` que lanza `NotImplementedError`, y subclases `Circulo`, `Rectangulo`, `Triangulo`. Recórrelas en una lista y muestra el área de cada una (polimorfismo).

### 72. Dunder methods — `72_vector.py`
Clase `Vector2D` con `__add__`, `__sub__`, `__mul__` (escalar), `__eq__`, `__abs__`, `__repr__`.

### 73. Baraja de cartas — `73_baraja.py`
Clases `Carta` y `Baraja` con `__len__`, `__getitem__`, barajar y repartir manos.

### 74. Atributos de clase — `74_contador.py`
Clase que lleve la cuenta de cuántas instancias se han creado, con un `@classmethod` que la devuelva y un `@staticmethod` auxiliar.

### 75. Dataclasses — `75_dataclass.py`
Reescribe el ejercicio 69 con `@dataclass`. Añade `field(default_factory=...)` y `frozen=True`, y observa qué cambia.

### 76. Biblioteca — `76_biblioteca.py`
`Libro`, `Usuario` y `Biblioteca`: prestar (validando disponibilidad), devolver, buscar por autor o título, listar préstamos activos. Guarda el estado en JSON.

---

## Nivel 10 — Python intermedio
*Módulos, `collections`, decoradores, generadores, comprensión del lenguaje.*

### 77. Tu propio módulo — `77_utilidades.py` + `77_usar_utilidades.py`
Crea un módulo con tus funciones favoritas de los niveles anteriores e impórtalo desde otro archivo.

### 78. `collections` — `78_collections.py`
Resuelve con `Counter`, `defaultdict`, `namedtuple` y `deque` cuatro problemas que ya resolviste a mano (42, 45, 41 y 16).

### 79. Decorador de tiempo — `79_decorador_tiempo.py`
`@cronometro` que mida cuánto tarda una función. Aplícalo a las dos versiones de Fibonacci del ejercicio 53. Usa `functools.wraps`.

### 80. Decorador con argumentos — `80_decorador_reintentos.py`
`@reintentar(veces=3, espera=1)` que reintente una función que falla aleatoriamente.

### 81. Generadores — `81_generadores.py`
Un generador infinito de Fibonacci, uno que lea un archivo línea a línea, y compara el uso de memoria frente a una lista con `sys.getsizeof`.

### 82. Context manager propio — `82_context_manager.py`
Con `contextlib.contextmanager`, crea uno que cronometre un bloque de código. Luego hazlo con `__enter__`/`__exit__`.

### 83. Type hints — `83_tipado.py`
Añade anotaciones de tipo completas a tu módulo del 77. Si puedes, instala `mypy` y corrige lo que reporte.

---

## Nivel 11 — Proyectos pequeños
*Integra todo. Cada uno debe tener funciones o clases, manejo de errores y persistencia.*

### 84. Juego del ahorcado — `84_ahorcado.py`
Palabra aleatoria desde un archivo, dibujo por estado, intentos, letras usadas.

### 85. Gestor de gastos — `85_gastos.py`
Registra gastos con fecha, categoría e importe. Resúmenes por mes y por categoría. Persistencia en CSV o JSON.

### 86. Cliente de API — `86_api_clima.py`
Consume una API pública (por ejemplo `https://api.open-meteo.com`) con `requests` o `urllib`, parsea el JSON y muestra un pronóstico formateado. Maneja errores de red.

### 87. Tres en raya — `87_tres_en_raya.py`
Dos jugadores, validación de jugadas, detección de victoria/empate. Extra: una IA simple que no pierda.

### 88. Tests con pytest — `88_test_utilidades.py`
Escribe tests para tu módulo del 77: casos normales, límites y errores esperados con `pytest.raises`.

### 89. CLI real — `89_cli_tareas.py`
Convierte el gestor de tareas (68) en una CLI con `argparse`:
`python 89_cli_tareas.py add "Comprar pan"` / `list --pendientes` / `done 3`.

---

## Qué reviso cuando me pases un ejercicio

- **¿Funciona?** Casos normales, vacíos y límites.
- **¿Es pythónico?** Nombres, idioms (`enumerate`, desempaquetado, comprensiones), evitar repetición.
- **¿Está bien estructurado?** Funciones con una responsabilidad, sin lógica suelta al nivel del módulo.
- **¿Maneja errores?** Entradas inválidas, división por cero, archivos que no existen.
- **¿Se lee bien?** Formato PEP 8, nombres claros, comentarios solo donde aportan.

Pásamelos de uno en uno o en tandas, como prefieras.
