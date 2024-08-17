# Analizador Léxico en JavaScript

Este es un simple analizador léxico implementado en HTML y JavaScript. El programa identifica los siguientes tokens en una cadena de texto:

- **Identificadores**: Secuencias de caracteres que comienzan con una letra y pueden continuar con letras o dígitos.
- **Números reales**: Números que contienen un punto decimal, con al menos un dígito antes y después del punto.

## Reglas de Identificación

- **Identificadores**: Se identifican usando la expresión regular `^[a-zA-Z][a-zA-Z0-9]*$`, que garantiza que comiencen con una letra (`a-z` o `A-Z`) y continúen con letras o dígitos (`0-9`).
- **Números reales**: Se identifican con la expresión regular `^\d+\.\d+$`, que busca un número entero seguido de un punto y otro número entero.

## Estructura del Proyecto

El proyecto consta de un único archivo HTML que contiene tanto el código HTML como el JavaScript necesario para el analizador.

### `index.html`

Este archivo incluye:

- Un campo de texto donde puedes ingresar el texto a analizar.
- Un botón para iniciar el análisis.
- Un área de resultados donde se muestran los tokens reconocidos.

### Funcionamiento

1. **Input**: El usuario ingresa una cadena de texto en el campo de entrada.
2. **Análisis**: El programa divide el texto en tokens utilizando espacios como delimitadores.
3. **Resultado**: Los tokens se clasifican como identificadores, números reales, o tokens no reconocidos y se muestran en la página.

## Uso

1. Descarga el archivo `index.html`.
2. Abre el archivo en cualquier navegador web.
3. Ingresa una cadena de texto en el campo de entrada.
4. Haz clic en "Analizar" para ver los resultados.

## Ejemplo de Entrada y Salida

### Entrada:
variable1 123.45 otroIdentificador 678.9

### Salida:
Identificador: variable1
Número Real: 123.45
Identificador: otroIdentificador
Número Real: 678.9




