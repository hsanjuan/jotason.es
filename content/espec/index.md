+++
title = 'Jotasón v1.0'
date = 2023-12-08T14:39:05+01:00
draft = false
weight = 1
+++

## Introducción

El formato jotasón sirve para encapsular estrofas de jota aragonesa de temática relacionada con la informática, la ingeniería del software, el *hacking* y otros campos próximos a estas disciplinas.

Los jotasones son fáciles de leer y de escribir. Un jotasón debe respetar tanto los formatos lexicográficos definidos en este estándar, como la temática y ortografía para palabras importadas de otras lenguas.

## Objeto Jotasón

Un jotasón es un objecto que comienza por `{` y acaba con `}` (corchetes) y que contiene una o varias *estrofas* indentadas por un tabulado y separadas por una línea vacía.

Tanto el corchete de apertura como el de cierre son el único caracter en la primera y última líneas y no presentan identación.

Ejemplo:

	{
		<estrofa 1>
	
		<estrofa 2>
	
		...
	}


### Estrofas

Las estrofas consisten en cuatro versos de arte menor correspondientes a los siguientes tipos:

  - Cuarteta: Cuatro versos (generalmete octosílabos) con rima consonante *8A 8B 8A 8B*.
  - Copla: Cuatro versos (generalmente octosílabos) con rima asonante *8- 8a 8- 8a* (romance) o *8a 8b 8a 8b* (redondilla).

Por ejemplo, el siguiente jotasón contiene una copla como estrofa:

	{
		Si te mandan jotasones
		parsea la petición,
		a menos que lleve el jéder
		pide la autenticación.
	}

### Idioma

Los versos de jotasón están escritos generalmente en idioma español aunque se aceptan otras lenguas y dialectos romances que funcionen con los tipos de estrofas permitidos.

#### Prestamos lexicos

Toda palabra no perteneciente al idioma principal del jotasón (extranjerismos) debe ser adaptada a las reglas de la lengua receptora, aunque en principio no existan en ella. Incluso si existe una traducción o palabra equivalente para un extranjerismo, se permite la adaptación y uso de la palabra original como parte de la licencia poética.

Normalmente es el caso de anglicismos, cuya pronunciación deberá quedar debidamente definida, aunque esta esté adaptada o difiera de la real en el idioma original.

Ejemplos:

  - *Hardware* -> hargüar
  - *Kernel* -> quérnel
  - *DDOS* -> dedós
  - *Autoscaling* -> autoesqueilin

### Temática

Un jotasón ha de tratar siempre sobre temas relacionados con la informática, la ingeniería del software, la inteligencia artifical, el hacking etc. El universo temático del jotasón es muy amplio pues la informática tiende puentes a otras temáticas poéticas como el amor, la justicia social o la historia.

Para temas no relacionados en absoluto se recomienda usar otros formatos poéticos como el soneto o la lira.

### Formato pretificado

El jotasón puede representarse en formato "pretificado" cuando los cuatro versos de sus estrofas se disponen a manera de jota aragonesa para su cante, con el verso 2 como entrada y final, y el verso 4 como vuelta en la siguiente disposición:

  1. Entrada (verso 2)
  2. Verso 1
  3. Verso 2
  4. Verso 3
  5. Verso 4
  6. Vuelta (verso 4)
  7. Final y mundanza (verso 1)

Por ejemplo, un jotasón pretificado sería el siguiente:

	{
		Parsea la petición, (2)
		si te mandan jotasones (1)
		parsea la petición, (2)
		a menos que lleve el jéder (3)
		pide la autenticación, (4)
		pide la autenticación (4)
		si te mandan jotasones. (1)
	}

Nótese que para que un jotasón sea pretificable ha de cuadrar el primer verso tanto con el segundo como con el cuarto. En en ejemplo, ambas frases tienen sentido: `Parsea la petición / si te mandan jotasones`, `Pide la autenticación / si te mandan jotasones`.
