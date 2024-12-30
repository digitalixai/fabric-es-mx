<div align="center">

<img src="https://beehiiv-images-production.s3.amazonaws.com/uploads/asset/file/2012aa7c-a939-4262-9647-7ab614e02601/extwis-logo-miessler.png?t=1704502975" alt="extwislogo" width="400" height="400"/>

# `/extractwisdom`

<h4><code>extractwisdom</code> es un patrón de<a href="https://github.com/danielmiessler/fabric" target="_blank">Fabric</a> que <em>extrae sabiduría </em> de cualquier texto.</h4>

[Description](#description) •
[Functionality](#functionality) •
[Usage](#usage) •
[Output](#output) •
[Meta](#meta)

</div>

<br />

## Descripción

**`extractwisdom` aborda el problema de **demasiado contenido** y muy poco tiempo.**

_No solo eso, sino que también es demasiado fácil olvidar lo que leemos, vemos o escuchamos._

Este patrón extrae sabiduría de cualquier contenido que pueda traducirse a texto, por ejemplo:

- Transcripciones de podcasts  
- Artículos académicos  
- Ensayos  
- Publicaciones de blogs  
- ¡En realidad, cualquier cosa que puedas convertir en texto!

## Funcionalidad

Cuando usas `extractwisdom`, extrae el siguiente contenido de la entrada:

- `IDEAS`  
  - Extrae las mejores ideas del contenido, es decir, aquello sobre lo que podrías haber tomado notas si lo hicieras manualmente.
- `QUOTES`  
  - Algunas de las mejores citas del contenido.
- `REFERENCES`  
  - Escritos externos, arte y otros contenidos mencionados positivamente durante el contenido que podrían valer la pena explorar.
- `HABITS`  
  - Hábitos de los ponentes que podrían valer la pena replicar.
- `RECOMMENDATIONS`  
  - Una lista de cosas que el contenido recomienda, incluyendo los hábitos de los ponentes.

### Casos de uso

La salida de `extractwisdom` puede ayudarte de varias formas, incluyendo:

1. `Filtrado por tiempo`<br />
   Te permite ver rápidamente si el contenido vale la pena para una revisión más profunda o no.
2. `Toma de notas`<br />
   Puede usarse como un sustituto para tomar notas manuales que consumen mucho tiempo.

## Uso

Puedes referenciar el contenido **sistema** y **usuario** de `extractwisdom` directamente de la siguiente manera:

### Extrae directamente el prompt del _sistema_


```sh
curl -sS https://github.com/danielmiessler/fabric/blob/main/extract-wisdom/dmiessler/extract-wisdom-1.0.0/system.md
```

### Pull the _user_ prompt directly

```sh
curl -sS https://github.com/danielmiessler/fabric/blob/main/extract-wisdom/dmiessler/extract-wisdom-1.0.0/user.md
```

## Salida

Aquí tienes un ejemplo abreviado de salida de `extractwisdom` (limitado a solo 10 elementos por sección).

```markdown
## RESUMEN:

El contenido presenta una conversación entre dos personas que abordan diversos temas, incluyendo la decadencia de la cultura occidental, la importancia de la belleza y la sutileza en la vida, el impacto de la tecnología y la inteligencia artificial, la resonancia de la poesía de Rilke, el valor de la lectura profunda y la relectura de textos, la naturaleza cautivadora de los escritos de Ayn Rand, el papel de la filosofía en la comprensión del mundo y la influencia de las drogas en la sociedad. También tocan temas como la creatividad, los periodos de atención y la importancia de la introspección.

## IDEAS:

1. La cultura occidental se percibe en decadencia debido a la pérdida de valores y la aceptación de la mediocridad.
2. Los medios masivos y la tecnología han contribuido a periodos de atención más cortos y una necesidad constante de estímulos.
3. La poesía de Rilke resuena por su enfoque en la belleza y el éxtasis en objetos cotidianos.
4. La sutileza se pasa por alto en la sociedad moderna debido a la sobrecarga sensorial.
5. La tecnología juega un papel significativo en la conformación de la música y el arte escénico.
6. Los hábitos de lectura han cambiado de lecturas profundas y repetitivas a consumir grandes cantidades de material nuevo.
7. Releer libros influyentes con la edad puede ofrecer nuevas perspectivas basadas en experiencias y sabiduría acumuladas.
8. La ficción puede ilustrar conceptos filosóficos a través de personajes y narrativas.
9. Muchos pensadores influyentes tienen formación en filosofía, lo que subraya su importancia en las habilidades de razonamiento.
10. La filosofía actúa como un puente entre la teología y la ciencia, planteando preguntas que ambas disciplinas buscan responder.

## CITAS:

1. "No necesariamente puedes pensar en las respuestas. Tienes que crear espacio para que lleguen a ti."
2. "Occidente está muriendo y nosotros la estamos matando."
3. "El sueño americano ha sido reemplazado por pornografía de mediocridad empaquetada en masa, animándonos a regodearnos como cerdos felices en nuestra propia insignificancia."
4. "Simplemente no hay muchas personas que tengan el coraje de ir más allá del consenso y explorar nuevas ideas."
5. "Empezaré a ver Netflix cuando haya leído toda la historia de la humanidad."
6. "Rilke veía belleza en todo... encuentra en una cosa pequeña una representación de todas las cosas hermosas."
7. "La vainilla es un sabor muy sutil... refleja la sobrecarga sensorial de la era moderna."
8. "Cuando memorizas capítulos [de la Biblia], toma algunos meses, pero realmente entiendes cómo están estructurados."
9. "A medida que envejeces, si hay libros que te conmovieron en tu juventud, vale la pena volver a leerlos."
10. "Ella [Ayn Rand] tomó una filosofía complicada y la encarnó de una manera con la que cualquiera podría identificarse."

## HÁBITOS:

1. Evitar el consumo de medios masivos para un compromiso más profundo con textos históricos e investigación personal.
2. Releer regularmente libros influyentes de la juventud para obtener nuevas perspectivas con la edad.
3. Practicar la lectura profunda en lugar de leer rápidamente o simplemente hojear material.
4. Memorizar capítulos o pasajes completos de textos importantes para una mejor comprensión.
5. Desconectarse de las redes sociales y los ciclos de noticias rápidas para procesos de pensamiento más enfocados.
6. Caminar largas distancias como forma de meditación y reflexión.
7. Crear espacio para que los pensamientos se solidifiquen a través de la introspección y la quietud.
8. Abrazar emociones como el dolor o la ira plenamente en lugar de reprimirlas.
9. Buscar experiencias variadas a través de diferentes carreras y estilos de vida.
10. Priorizar la investigación impulsada por la curiosidad sin metas o restricciones específicas.

## HECHOS:

1. Occidente se percibe en decadencia debido a cambios culturales que se alejan de los valores tradicionales.
2. Los periodos de atención se han acortado debido a los avances tecnológicos y los hábitos de consumo mediático.
3. La poesía de Rilke enfatiza encontrar belleza en los objetos cotidianos a través de la observación detallada.
4. La sutileza se pasa por alto en la sociedad moderna debido a la sobrecarga sensorial de diversos estímulos.
5. Los hábitos de lectura han evolucionado de un compromiso profundo con los textos a consumir grandes cantidades rápidamente.
6. Releer libros influyentes puede ofrecer nuevas perspectivas basadas en experiencias de vida acumuladas.
7. La ficción puede ilustrar conceptos filosóficos de manera efectiva a través del desarrollo de personajes y arcos narrativos.
8. La filosofía juega un papel significativo en el desarrollo de habilidades de razonamiento y comprensión de ideas complejas.
9. La creatividad puede verse obstaculizada por el nihilismo cultural y actitudes proteccionistas dentro de la sociedad.
10. El pensamiento a corto plazo socava los esfuerzos por crear obras duraderas de belleza o significado.

## REFERENCIAS:

1. Poesía de Rainer Maria Rilke  
2. Netflix  
3. Concierto de Underworld  
4. Actuaciones teatrales de Katy Perry  
5. Actuaciones de Taylor Swift  
6. Estudio bíblico  
7. "La rebelión de Atlas" de Ayn Rand  
8. Escritos de Robert Pirsig  
9. Definición de filosofía de Bertrand Russell  
10. Caminatas de Nietzsche  