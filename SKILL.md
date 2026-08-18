---
name: skill-guia-estilo-informe-tecnico
description: Aplica cuando se redacta, revisa o corrige un informe técnico/académico en LaTeX. Úsala al escribir contenido nuevo, al revisar un borrador existente, o cuando el usuario pida "revisar el informe", "corregir estilo", "dar formato al TFG/memoria", o mencione títulos, figuras, tablas, metodología, referencias cruzadas o maquetado de un documento técnico. Impone reglas concretas de redacción, tipografía, figuras, tablas y estructura basadas en correcciones reales de un profesor/revisor académico.
---

# Guía de estilo para informes técnicos

Checklist normativo para escribir y revisar informes técnicos/académicos. No es un conjunto de sugerencias:
son correcciones reales que un revisor ya ha marcado como errores, así que al redactar
o revisar contenido hay que aplicarlas de forma activa, no solo mencionarlas.

## Cuándo usar esta skill

- El usuario pide escribir, ampliar o reescribir secciones de un informe técnico.
- El usuario pide "revisar", "corregir" o "dar el visto bueno" a un borrador (LaTeX,
  Word, Markdown convertido a informe, etc.).
- Se está maquetando o cerrando la versión final antes de entrega.
- Se generan figuras, tablas o ecuaciones que van a insertarse en el documento.

Si el trabajo no es un informe técnico/académico formal (por ejemplo, documentación de
código, un README, un email), esta skill no aplica.

## Cómo trabajar

1. Si estás revisando un documento existente, recorre el checklist del final de la skill punto por punto y
   señala cada incumplimiento con su ubicación exacta (sección, página o número de
   línea/figura).
2. Si estás redactando contenido nuevo, aplica las reglas directamente al escribir; no
   generes texto que luego haya que corregir.
3. Cuando una regla obligue a reestructurar (p. ej. mover una referencia cruzada antes
   de la figura), hazlo tú mismo si tienes permiso de edición; si solo estás revisando,
   indícalo explícitamente como acción pendiente.
4. Ante ambigüedad entre "menos es más" y "que no falte nada necesario", prioriza
   siempre la comprensión del lector: elimina lo redundante, nunca lo imprescindible.

---

## 0. Estructura global del informe

Todo informe debe presentar, antes de nada:

- **Portada** con título, autores, fecha, y encuadre del trabajo (asignatura, grado/máster,
  titulación).
- **Índice de contenidos** con todas las secciones y subsecciones.

El cuerpo del documento debe seguir siempre este esqueleto mínimo, en este orden:

1. Resumen y palabras clave
2. Introducción
3. Metodología
4. Resultados
5. Conclusiones y futuros trabajos
6. Bibliografía

Es flexible: se pueden añadir secciones, subsecciones o anexos adicionales si el trabajo lo
requiere (revisión de literatura, marco teórico, configuración de equipos, etc.), pero
ninguno de estos seis bloques puede faltar.

## Resumen y palabras clave

- Extensión: 250-300 palabras.
- Debe explicitar tres cosas: qué problema se resuelve, cómo se ha resuelto y qué
  conclusiones principales se han extraído.
- Nunca debe incluir referencias bibliográficas.
- Se redacta al final del proceso de escritura del documento, no al principio.
- Palabras clave: 6 recomendadas.

## 1. Introducción

La introducción debe incluir explícitamente:

- **Planteamiento del problema**: qué carencia, necesidad o pregunta motiva el trabajo.
- **Planteamiento de la solución**: qué se ha hecho para abordarlo.
- **Material y medios empleados**: con qué se ha resuelto (herramientas, datos, equipo,
  entorno).
- **Mapa del documento**: al final de la introducción, describir la estructura del resto del
  documento haciendo referencia cruzada a cada sección posterior, para que el lector sepa
  dónde encontrar cada contenido.

Si falta alguno de estos cuatro bloques, la introducción está incompleta aunque el texto
"suene bien".

## 2. Capitalización de títulos

- Títulos de secciones y subsecciones: **minúsculas**, salvo la primera letra de la
  primera palabra y los nombres propios.
- Incorrecto: `Análisis De Resultados Del Sistema`
- Correcto: `Análisis de resultados del sistema`
- Los nombres propios (marcas, algoritmos con nombre propio, lugares, personas, siglas)
  mantienen su mayúscula donde corresponda: `Resultados del ensayo con Arduino`.

## 3. Uso mínimo pero suficiente de figuras

- Minimizar el número de figuras: cada figura debe justificar su presencia.
- Nunca eliminar una figura que sea imprescindible para el contexto o la comprensión
  del resultado solo por reducir el conteo.
- Antes de insertar una figura, pregúntate: ¿el texto o una tabla podrían transmitir lo
  mismo con igual claridad? Si sí, prescinde de la figura.

## 4. Epígrafes (captions) de figuras

- Nunca terminan en punto final.
- Evitar el uso de "vs." en el epígrafe (y en general en el cuerpo del texto); usar
  "frente a" o reformular.

## 5. Índices de figuras y tablas

- Si el documento no contiene figuras, no incluir un índice de figuras (y análogamente
  para tablas). Un índice vacío o de un único elemento no aporta nada.
- **Nunca** un índice de figuras/tablas dentro de una sección de resultados numéricos:
  eso no es su lugar.

## 6. Negrita dentro de párrafos

- No usar negrita para enfatizar frases o resultados dentro de un párrafo de un informe
  técnico. El énfasis se logra con la redacción, no con formato tipográfico.
- Excepción explícita: los encabezados en negrita de los puntos de la metodología (ver
  regla 7).

## 7. Estructura fija del apartado de Metodología

El apartado de Metodología sigue siempre esta estructura:

1. **Párrafo introductorio breve** que anuncia que se van a enumerar los pasos
   metodológicos seguidos para resolver el problema planteado. Ejemplo de tono:

   > Para dar solución al problema descrito y estructurar los ensayos de este trabajo,
   > se han seguido los siguientes pasos metodológicos:

2. **Un bullet/punto por cada sección principal del cuerpo del trabajo**, en el mismo
   orden en que aparecen después, **excepto** las secciones de bibliografía y
   conclusiones (esas no se listan en la metodología).
   - Formato de cada punto: el nombre de la sección **en negrita**, seguido de dos
     puntos y una breve explicación de qué se va a ver/hacer en ese punto.

   Ejemplo: si el trabajo tiene después las secciones "Obtención de datos",
   "Experimento práctico" y "Evaluación de resultados", la metodología queda:

   ```
   1) Obtención de datos: se describe el origen de los datos utilizados y el
      procedimiento seguido para su recopilación.
   2) Experimento práctico: se detalla el montaje y la ejecución de los ensayos
      realizados sobre el sistema.
   3) Evaluación de resultados: se analizan los resultados obtenidos y se
      contrastan con los objetivos planteados.
   ```

   Solo el nombre de la sección va en negrita; la explicación va en texto normal (esto
   no contradice la regla 6, que prohíbe la negrita de énfasis dentro de párrafos
   corridos, no en encabezados de lista).

Al revisar un informe, comprueba que la lista de la metodología case exactamente con
las secciones reales del documento (mismo orden, mismos nombres, sin bibliografía ni
conclusiones).

## Resultados

- Las subsecciones de "Resultados" deben corresponder 1:1, y en el mismo orden, con los
  puntos numerados de la lista de "Metodología" (ver regla 7).
- Todo resultado numérico, gráfico o tabla debe comentarse y analizarse explícitamente en el
  texto; no debe quedar una figura o tabla sin comentar.

## Conclusiones y futuros trabajos

- Deben recopilar los comentarios y conclusiones parciales ya escritos en "Resultados", más
  una conclusión final de cierre.
- Deben enunciar mejoras y líneas de trabajo futuro, indicando si ya se está trabajando en
  alguna de ellas.

## Bibliografía: fuentes admisibles

- Prohibido citar la Wikipedia, o usar figuras extraídas de ella.
- Prohibido citar webs sin prestigio reconocido; solo se admiten fuentes de prestigio (IEEE,
  ISA, Elsevier, editoriales/journals académicos, datasheets oficiales, etc.).

## Consideraciones generales de redacción

- Cada párrafo debe tener entidad suficiente: al menos ~6 líneas siempre que sea posible; no
  dejar párrafos de una sola frase suelta.
- Redacción preferiblemente impersonal; se permite ocasionalmente la 1ª persona del plural
  ("hemos comprobado que...", "en este trabajo se ha analizado...").
- Los títulos de sección y subsección nunca terminan en punto.
- Nunca debe existir una única subsección suelta dentro de una sección: si se crea una
  subsección, debe haber al menos dos, o ninguna.
- Toda sección/subsección debe contener al menos un párrafo de texto antes de su primera
  subsección; no se puede saltar directamente al primer subapartado.

## 8. Orden de las referencias cruzadas respecto a las figuras

- La referencia cruzada a una figura (p. ej. "como se observa en la figura 3...") debe
  aparecer **siempre antes** de la propia figura en el flujo del documento.
- Nunca insertar una figura y comentarla/referenciarla después de que ya haya
  aparecido.
- Al revisar, verifica el orden real de aparición en el PDF compilado, no solo el orden
  en el código fuente (los flotantes de LaTeX pueden desplazarse).
- Nunca usar fórmulas como "en la siguiente figura/tabla...": la referencia a una figura o
  tabla debe hacerse siempre mediante referencia cruzada (p. ej. "como se puede ver en la
  figura 3"), no mediante una alusión posicional.
- Rótulo obligatorio: en figuras, "Figura" con el título situado debajo de la imagen; en
  tablas, "Tabla" con el título situado encima de la tabla.

## 9. Resolución y formato de las figuras

- Las figuras deben estar en formato vectorial: **EPS o PDF** (nunca rasterizado tipo
  PNG/JPG de baja resolución para gráficas o diagramas generados por el propio autor).
- Excepción razonable: capturas de pantalla de software de terceros que no se pueden
  regenerar en vectorial; en ese caso, usar la mayor resolución disponible.

## 10. Maquetado final

- Antes de dar por cerrado el documento, revisar el PDF compilado completo, página por
  página.
- No puede quedar una página con la mitad en blanco a mitad del trabajo por culpa de
  una figura grande que se desplaza a la página siguiente (float de LaTeX mal ubicado).
- Soluciones típicas: usar `[!htbp]`/`[H]` con criterio, reordenar el texto,
  redimensionar la figura, o mover el flotante a una página de figuras dedicada (ver
  regla 14).

## 11. Enfoque en la región de interés de gráficas de resultados

- En gráficas de análisis de resultados (curvas temporales, comparativas, etc.), el eje
  y los límites deben centrarse en la región de interés.
- Si una parte de la gráfica es irrelevante para la conclusión que se quiere mostrar
  (tramos planos, transitorios sin interés, rangos fuera de escala), recórtala o
  ajusta los límites de los ejes en vez de mostrar la curva completa "porque sí".
- Esta regla solo aplica cuando existe efectivamente una parte irrelevante; no recortar
  gráficas que ya son enteramente relevantes.

## 12. Formato de tablas: estilo "booktabs"

- Todas las tablas deben usar el estilo `booktabs` (líneas horizontales `\toprule`,
  `\midrule`, `\bottomrule`; sin líneas verticales; sin doble línea).
- No usar cuadrículas completas ni líneas verticales entre columnas.

## 13. Fuente y cita de figuras no propias

- Si una figura no es de elaboración propia (capturas, gráficos de otros autores,
  diagramas de datasheets, imágenes de internet), se debe:
  - Indicar la fuente en el propio epígrafe (p. ej. "Fuente: [12]" o "Adaptado de
    [12]").
  - Incluir la referencia bibliográfica correspondiente en la bibliografía.
  - Si la fuente es una web, indicar también la fecha de consulta.
- Las figuras de elaboración propia no necesitan esta atribución.

## 14. Consistencia y agrupación de figuras repetitivas

Cuando el informe presenta muchas figuras estructuralmente similares (p. ej. la misma
pareja de gráficas "acción de control en x" / "acción de control en y" frente al
tiempo, repetida para varias configuraciones o ensayos):

- Fijar un **tamaño consistente** para todas las figuras de ese tipo a lo largo del
  documento; no dejar que unas sean grandes y otras pequeñas sin motivo.
- Evitar figuras sueltas, muy aisladas o desproporcionadamente grandes para su
  contenido.
- Agrupar las figuras similares en **páginas de flotantes**, preferiblemente de
  cuatro en cuatro (2x2), cuando correspondan al mismo formato de comparación mostrado
  sobre distintos ensayos/configuraciones.
- Cada página de figuras agrupadas debe tener su propia referencia cruzada desde el
  texto (regla 8) donde se comenten en conjunto los resultados mostrados.
- Además, usar una paleta de colores uniforme y suave (sin estridencias) en todas las
  figuras del documento, no solo el mismo tamaño.

## 15. Numeración de ecuaciones

- Numerar **solo** las ecuaciones a las que se va a hacer referencia cruzada en algún
  punto del texto.
- Las ecuaciones que no se citan en ningún otro lugar del documento van sin número
  (p. ej. `\begin{equation*}` o `\[ ... \]` en LaTeX, no `\begin{equation}`).
- Las ecuaciones **nunca** deben ser imágenes o capturas (de webs, PDFs o libros escaneados):
  siempre se escriben con la sintaxis matemática de LaTeX.
- La referencia cruzada a una ecuación numerada va **después** de que esta aparezca en el
  texto (al contrario que en figuras/tablas, donde la referencia va antes; ver regla 8).
- Las deducciones matemáticas largas no se transcriben paso a paso completas: solo se
  explicitan los pasos clave, indicando en el texto cómo se ha llegado al resultado.
- El símbolo de producto entre variables o cantidades nunca es el asterisco `*`; usar
  yuxtaposición, `\,`, `\cdot` o `\times`.
- Unidades de medida: siempre con espacio entre la cantidad y la unidad, y la unidad en tipo
  redondo (nunca en cursiva).
- Separador decimal: coma o punto son válidos; se prefiere la coma.

---

## Checklist rápido de revisión

Al revisar un informe ya escrito, recorre esta lista y reporta cada incumplimiento con
su ubicación:

- [ ] Portada e índice de contenidos presentes
- [ ] Estructura mínima completa: resumen+palabras clave, introducción, metodología,
      resultados, conclusiones y futuros trabajos, bibliografía
- [ ] Resumen de 250-300 palabras, con problema+solución+conclusiones, sin bibliografía, y
      6 palabras clave
- [ ] Introducción: problema + solución + material/medios + mapa del documento con
      referencias cruzadas
- [ ] Subsecciones de "Resultados" correspondientes 1:1 con los puntos de la metodología
- [ ] Todo resultado/gráfico/tabla comentado explícitamente en el texto
- [ ] Conclusiones recogen lo dicho en resultados y enuncian trabajos futuros
- [ ] Bibliografía sin Wikipedia ni webs de dudoso prestigio
- [ ] Párrafos con entidad suficiente (~6 líneas), redacción impersonal
- [ ] Ninguna subsección suelta (única) dentro de una sección
- [ ] Toda sección tiene un párrafo antes de su primera subsección
- [ ] Títulos en minúsculas salvo inicial y nombres propios; sin punto final
- [ ] Ninguna figura prescindible; ninguna figura imprescindible eliminada
- [ ] Epígrafes sin punto final; sin "vs."
- [ ] Sin índice de figuras/tablas si no hay contenido para él
- [ ] Sin negrita de énfasis en párrafos corridos
- [ ] Metodología con párrafo intro + bullets numerados por sección (sin biblio/conclusiones)
- [ ] Toda referencia cruzada de figura/tabla aparece antes que su figura; sin "en la
      siguiente figura..."
- [ ] Rótulo "Figura" (título abajo) / "Tabla" (título arriba) correcto
- [ ] Figuras en EPS/PDF vectorial
- [ ] Sin páginas con hueco en blanco por floats mal ubicados
- [ ] Gráficas de resultados centradas en la región de interés
- [ ] Tablas en estilo booktabs
- [ ] Figuras ajenas con fuente citada, fecha de consulta si es web, y referencia en
      bibliografía
- [ ] Figuras repetitivas con tamaño y paleta de colores consistentes, agrupadas en páginas
      de 4
- [ ] Solo ecuaciones referenciadas están numeradas; ninguna ecuación es una imagen/captura
- [ ] Referencia cruzada a ecuación aparece después de la ecuación
- [ ] Sin asterisco como símbolo de producto; unidades con espacio y en redonda
