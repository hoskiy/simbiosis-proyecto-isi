# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Fecha | [dd/mm/aaaa] |
| Versión | [Versión de trabajo] |
| Estado | Borrador |

## Fuentes comunes

- [Acta de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.
- [Catálogo de requisitos](catalogo-requisitos.md), UR-08 y FR pertinentes.
- [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), UC-21.

## Épica de búsqueda

Como usuario, quiero poder añadir criterios, para buscar recetas.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta.

## Justificación de la división

Añadir criterios es demasiado amplio, se debe concretar las diferentes formas de hacerlo

## US-01

**Título:** Buscar mediante texto

Como usuario, quiero poder buscar recetas una palabra o frase, para localizar recetas que coincidan con ella.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, acuerdos.

### Criterios de aceptación

- **CA-01.** Dado una búsqueda, cuando se haya añadido una palabra o frase, entonces solo se mostraran recetas que coincidan.
- **CA-02.** Dado una búsqueda sin resultados, cuando el texto tenga errores ortográficos, entonces el sistema propondrá una corrección.
- **CA-03.** Dado una búsqueda sin resultados, cuando el texto no tenga errores ortográficos, entonces el sistema propondrá alternativas relacionadas con los criterios.

## US-02

**Título:** Buscar por ingredientes incluidos

Como usuario, quiero poder incluir ingredientes, para buscar recetas que los contengan.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, acuerdos.

### Criterios de aceptación

- **CA-01.** Dado una búsqueda, cuando haya ingredientes incluidos, entonces solo se mostraran recetas que contengan todos los ingredientes seleccionados.
- **CA-02.** Dado una búsqueda, cuando alguno de los ingredientes incluidos también esté excluido, entonces el sistema avisará al usuario para que corrija el conflicto.
- **CA-03.** Dado [situación], cuando [acción], entonces [resultado observable].

## US-03

**Título:** Excluir ingredientes

Como usuario, quiero poder excluir ingredientes, para buscar recetas que no los incluyan.

**Fuentes:** UR-08; UC-21; [FR principal]; acta, acuerdos.

### Criterios de aceptación

- **CA-01.** Dado una busqueda, cuando haya ingredientes excluidos, entonces solo se mostraran recetas que no contengan esos ingredientes.
- **CA-02.** Dado una búsqueda, cuando alguno de los ingredientes excluidos también esté incluido, entonces el sistema avisará al usuario para que corrija el conflicto.
- **CA-03.** Dado [situación], cuando [acción], entonces [resultado observable].

## Revisión INVEST

La revisión abarca US-01, US-02 y US-03. «Aplicado» indica si se ha realizado la comprobación. «Cumple» indica si todas las historias cumplen el criterio. Si alguna no lo cumple, indicar «No» e identificar la historia y el motivo en la justificación. Si no se ha realizado la comprobación o faltan datos, indicar «Pendiente» en «Cumple».

| Criterio | Pregunta de revisión | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- | --- |
| Independiente | ¿Puede implementarse cada historia y ofrecer un resultado útil sin implementar antes las otras historias del conjunto? Puede compartir infraestructura con ellas. | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Negociable | ¿Cada historia explica qué necesita la persona y deja margen para discutir los detalles de la solución, respetando los acuerdos confirmados? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Valiosa | ¿La parte «para…» de cada historia explica el beneficio que obtiene la persona al usar esa capacidad? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Estimable | ¿Están claros el alcance y los datos necesarios para estimar el trabajo de cada historia? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Pequeña | ¿Se centra cada historia en una única capacidad de alcance manejable? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |
| Comprobable | ¿Los criterios de aceptación de cada historia describen acciones y resultados observables que permiten distinguir un comportamiento correcto de uno incorrecto? | [Sí/No] | [Sí/No/Pendiente] | [Historias y motivo] |

## Dudas pendientes

[Cuestiones pendientes de aclaración. Si no quedan cuestiones, indicar «Ninguna».]
