# Práctica interactiva de pruebas de hipótesis

Aplicación web educativa para practicar **pruebas de hipótesis sobre la media y la varianza**, desarrollada como material de apoyo para estudiantes de **Gestión Empresarial**.

La herramienta busca que el estudiante no se limite a sustituir valores en fórmulas, sino que comprenda el proceso completo de una prueba de hipótesis: identificar el parámetro de interés, seleccionar la distribución adecuada, formular las hipótesis, determinar la dirección de la prueba, interpretar regiones críticas, valores-p e intervalos de confianza, y finalmente expresar una conclusión en el contexto del problema.

## Características principales

- Banco de **157 reactivos**.
- **15 preguntas aleatorias por intento**.
- Selección balanceada de temas.
- **6 preguntas gráficas por intento**.
- Gráficas generadas mediante **Canvas**.
- Preguntas interactivas para seleccionar:
  - cola izquierda;
  - cola derecha;
  - ambas colas.
- La región seleccionada por el estudiante se representa gráficamente antes de calificar.
- **Modo estudio** con retroalimentación inmediata.
- Modo de evaluación sin mostrar la respuesta antes de calificar.
- Explicaciones breves después de cada reactivo.
- Opción para repasar únicamente las respuestas incorrectas.
- Generación de reporte imprimible y exportable como PDF.
- Registro del nombre del estudiante, intento y calificación.
- Diseño responsive para computadora, tableta y dispositivos móviles.
- Funciona completamente **offline**.
- No utiliza librerías externas.

## Contenido

La práctica incluye pruebas de hipótesis para:

### Media con distribución z

Se utiliza cuando se estudia la media poblacional y la desviación estándar poblacional `σ` es conocida.

\[
z=\frac{\bar{x}-\mu_0}{\sigma/\sqrt{n}}
\]

### Media con distribución t de Student

Se utiliza cuando se estudia la media poblacional, `σ` es desconocida y se utiliza la desviación estándar muestral `s`.

\[
t=\frac{\bar{x}-\mu_0}{s/\sqrt{n}}
\]

con:

\[
gl=n-1
\]

### Varianza con distribución χ²

Se utiliza para realizar inferencia sobre una varianza poblacional, bajo el supuesto correspondiente de normalidad.

\[
\chi^2=\frac{(n-1)s^2}{\sigma_0^2}
\]

con:

\[
gl=n-1
\]

## Habilidades que se practican

Los reactivos permiten trabajar, entre otros, los siguientes aspectos:

- identificación del parámetro de interés;
- selección entre pruebas z, t y χ²;
- planteamiento de \(H_0\) y \(H_1\);
- identificación de pruebas de cola izquierda, derecha y bilateral;
- ubicación de regiones críticas;
- cálculo del estadístico de prueba;
- toma de decisiones mediante región crítica;
- interpretación del valor-p;
- interpretación gráfica del valor-p;
- construcción e interpretación de intervalos de confianza;
- límites de confianza unilaterales;
- relación entre pruebas de hipótesis e intervalos de confianza;
- conclusiones redactadas en el contexto del problema.

## Relación entre la hipótesis alternativa y las colas

Una idea central de la práctica es que la dirección de la prueba se determina a partir de la hipótesis alternativa:

| Hipótesis alternativa | Tipo de prueba |
|---|---|
| \(H_1:\theta<\theta_0\) | Cola izquierda |
| \(H_1:\theta>\theta_0\) | Cola derecha |
| \(H_1:\theta\neq\theta_0\) | Dos colas |

Los reactivos utilizan expresiones contextualizadas como:

- aumentó;
- disminuyó;
- es mayor;
- es menor;
- cambió;
- es diferente.

## Pruebas χ² e intervalos de confianza

La aplicación dedica algunos reactivos específicamente a una confusión frecuente en pruebas de varianza.

En una **prueba de hipótesis**:

- una varianza muestral grande produce un estadístico χ² grande;
- una varianza muestral pequeña produce un estadístico χ² pequeño.

Por tanto:

\[
H_1:\sigma^2>\sigma_0^2
\Rightarrow
\text{cola derecha}
\]

\[
H_1:\sigma^2<\sigma_0^2
\Rightarrow
\text{cola izquierda}
\]

Sin embargo, al construir un **intervalo de confianza para \(\sigma^2\)** se despeja la varianza poblacional a partir de:

\[
\frac{(n-1)s^2}{\sigma^2},
\]

por lo que los valores críticos de χ² aparecen de manera inversa en los límites del intervalo.

Los reactivos incluyen preguntas destinadas específicamente a distinguir ambos razonamientos.

## Contextos de los problemas

Los ejercicios están orientados principalmente a situaciones relacionadas con **Gestión Empresarial**, por ejemplo:

- ventas;
- costos;
- tiempos de atención;
- tiempos de entrega;
- servicio al cliente;
- cobranza;
- logística;
- devoluciones;
- satisfacción del cliente;
- comportamiento de procesos administrativos y comerciales.

También se conservan algunos contextos generales de procesos y operaciones cuando resultan apropiados para ilustrar los conceptos estadísticos.

## Estructura de cada intento

Cada intento contiene 15 reactivos seleccionados aleatoriamente del banco de 157 preguntas.

La selección está controlada para evitar que un intento quede concentrado únicamente en un tema. Se busca combinar preguntas relacionadas con:

- media con z;
- media con t;
- varianza con χ²;
- selección de prueba;
- hipótesis;
- dirección de la prueba;
- cálculo;
- regiones críticas;
- valor-p;
- intervalos de confianza;
- interpretación y conclusiones.

Además, cada intento contiene 6 reactivos con representación gráfica.

## Modo estudio

Al activar **Modo estudio**, la aplicación proporciona retroalimentación inmediatamente después de seleccionar una respuesta.

Se muestra:

- si la respuesta es correcta o incorrecta;
- la respuesta correcta;
- una breve explicación conceptual.

Este modo está pensado para utilizar la herramienta como material de práctica y autoestudio.

## Modo de evaluación

Con el modo estudio desactivado, las respuestas no se califican inmediatamente.

El estudiante responde las 15 preguntas y posteriormente selecciona:

**Calificar intento**

La aplicación muestra entonces:

- número de respuestas correctas;
- porcentaje obtenido;
- desempeño por tema;
- respuestas correctas e incorrectas;
- explicaciones de cada reactivo.

## Reporte

Después de calificar un intento puede generarse un reporte que incluye:

- nombre del estudiante;
- fecha;
- número de intento;
- calificación;
- pregunta;
- respuesta seleccionada;
- respuesta correcta;
- explicación;
- gráficas correspondientes.

El reporte puede guardarse como PDF utilizando la opción de impresión del navegador.

## Tecnologías utilizadas

El proyecto está desarrollado únicamente con:

- HTML5;
- CSS;
- JavaScript;
- Canvas API.

No utiliza frameworks, bibliotecas externas ni conexión a Internet.

Todo el proyecto está contenido en **un único archivo HTML**.

## Ejecución

No requiere instalación.

1. Descargar el archivo HTML.
2. Abrirlo con cualquier navegador moderno.
3. Escribir el nombre del estudiante.
4. Resolver el intento.
5. Seleccionar **Calificar intento**.
6. Opcionalmente generar el reporte en PDF.

## Uso educativo

Esta herramienta está diseñada como complemento para cursos introductorios de **Probabilidad y Estadística**, particularmente para estudiantes de Gestión Empresarial.

Su propósito es favorecer el razonamiento estadístico y la comprensión conceptual de las pruebas de hipótesis, no sustituir la explicación teórica, el desarrollo algebraico ni la discusión de los supuestos de cada procedimiento.

## Autor

Material educativo desarrollado para la enseñanza de Probabilidad y Estadística.
