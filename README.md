Emerald
=======


## Consideraciones Léxicas

A continuación se presentan las palabras reservadas del lenguaje. Éstas no pueden ser utilizadas como identificadores ni redefinidas.

---
boolbasaur    charizard    intmonchan    floatzel    voidporeon   onix    
registeer     unown        true          false       const        var
for           from         to            by          while        return
if            elsif        else          read        print        BOOM
tag           continue     switch        case        default       
---
Un identificador es una secuencia de caracteres alfanúmericos y el símbolo `_`, que empieza con una letra. Emerald es sensible a mayúsculas, 
por lo tanto los identificadores `Ejem`, `ejem` y `eJEm` son diferentes.

Los enteros (`intmonchan`) se representan con una secuencia de dígitos del `0` al `9`.

Los floats (`floatzel`) empiezan con una secuencia de dígitos, luego seguida por un punto y termina con otra secuencia de dígitos. 
Por ejemplo, `0.28`, `28.0` son números válidos pero `.28` y `28.` no.

Las cadenas de caracteres (`onix`) son una secuencia de caracteres ASCII entre comillas dobles. 
Por ejemplo: "Emerald FTW", "pokemon", "Hola!"

Un comentario simple (de una linea) son representados de la siguiente manera:
   # Hola, éste es un comentario de una línea.

Un comentario de varias lineas se representa así: 
      /* Éste es comentario de varias
         lineas en el lenguaje Emerald.
         Es muy chévere. */




## Tipos Escalares

* boolbasaur - bool
* charizard  - char
* intmonchan - int
* floatzel   - float

## Tipos Colección

* onix - string
* tipo arreglo[N..M]

## Tipos Estructurados

* registeer - register
* **ejemplo**: registeer REG { int campo1 := 0; int campo2; }
* **ejemplo acceder al campo**: REG.campo1  
* unown - union

## Vacío

* voidporeon - void

## Selector

* if () {...}
* if () INST;
* if () {...} else {...}
* if () {...} else if () {...}
* if () {...} else if () {...} else {...}

## Iteraciones

* for VAR from INIC to FIN {...}
* for VAR from INIC to FIN by SALTO {...}
* while () {...}

## Entrada/Salida

* read ???
* print 

## Operadores
_En orden de precedencia_

* \! \  - unario
* \^
* \* \  / \ %
* \+ \  - 
* \< \  <=  \  >=  \  > 
* \= \  !=
* \&&
* \||

## Asignación

* :=

## Declaración e Inicialización de Variables

### Pasado por Valor

* int V1, V2;
* int V3;
* int V4, V5 := 0, 1;
* int V6 := 2;

### Pasado por Referencia

* int var V1, var V2;
* int var V3;

## Comentarios

* \# una línea
* /* */ 

## Etiquetas

* etiqueta:
* BOOM - break
* BOOM etiqueta - break 
* continue etiqueta
* continue

## Case

* switch (EXPR) { case VALOR -> BLOQUE; default -> BLOQUE; }
* switch (EXPR) { case VALOR -> BLOQUE; }
* Los rangos son disjuntos
