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

## 1. Introducción

La introducción debe incluir explícitamente:

- **Planteamiento del problema**: qué carencia, necesidad o pregunta motiva el trabajo.
- **Planteamiento de la solución**: qué se ha hecho para abordarlo.
- **Material y medios empleados**: con qué se ha resuelto (herramientas, datos, equipo,
  entorno).

Si falta alguno de estos tres bloques, la introducción está incompleta aunque el texto
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

## 8. Orden de las referencias cruzadas respecto a las figuras

- La referencia cruzada a una figura (p. ej. "como se observa en la figura 3...") debe
  aparecer **siempre antes** de la propia figura en el flujo del documento.
- Nunca insertar una figura y comentarla/referenciarla después de que ya haya
  aparecido.
- Al revisar, verifica el orden real de aparición en el PDF compilado, no solo el orden
  en el código fuente (los flotantes de LaTeX pueden desplazarse).

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

## 15. Numeración de ecuaciones

- Numerar **solo** las ecuaciones a las que se va a hacer referencia cruzada en algún
  punto del texto.
- Las ecuaciones que no se citan en ningún otro lugar del documento van sin número
  (p. ej. `\begin{equation*}` o `\[ ... \]` en LaTeX, no `\begin{equation}`).

---

## Checklist rápido de revisión

Al revisar un informe ya escrito, recorre esta lista y reporta cada incumplimiento con
su ubicación:

- [ ] Introducción: problema + solución + material/medios
- [ ] Títulos en minúsculas salvo inicial y nombres propios
- [ ] Ninguna figura prescindible; ninguna figura imprescindible eliminada
- [ ] Epígrafes sin punto final; sin "vs."
- [ ] Sin índice de figuras/tablas si no hay contenido para él
- [ ] Sin negrita de énfasis en párrafos corridos
- [ ] Metodología con párrafo intro + bullets numerados por sección (sin biblio/conclusiones)
- [ ] Toda referencia cruzada aparece antes que su figura
- [ ] Figuras en EPS/PDF vectorial
- [ ] Sin páginas con hueco en blanco por floats mal ubicados
- [ ] Gráficas de resultados centradas en la región de interés
- [ ] Tablas en estilo booktabs
- [ ] Figuras ajenas con fuente citada y referencia en bibliografía
- [ ] Figuras repetitivas con tamaño consistente y agrupadas en páginas de 4
- [ ] Solo ecuaciones referenciadas están numeradas
