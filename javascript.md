Els comentaria amb JS es fan:

```js
// una linea de comentari

/*
varies lines
de comentaris
 */
```
 
# Tipus Valors primitius:

## string = cadea de text. 
```js
'hola',"hola","d'acord",  "l'autor va dir:\"caca\".",  

"aquesta es la lista: " + 
" - tronja" +
" - poma" +
" - melo" 

`aquesta es la lista:
 - tronja
 - poma
 - melo `
```

## Numeros 
```js
2 // = numero

'2' // = texto
```

## null = si sabem valor pero no es res

## undefined = no sabem valor

## Array : llista 
[1,2,3,'text',{}]
new Array(1,2,3...)
array[index]

## Object : diccionari amb valors
{a:1, b: 'text'}
new Object()

objecte.valor

## Boolean = true/false
true
false
new Boolean()

## Symbol = crear claus unicas
Symbol('caca') === Symbol('caca') // false

# Variables
var a = 1 - variable no respecta els blocs "blocs= part de codi expresada amb{}"
let b =2 - varible que respecta el bloc reasignable
const c= 3 - varible que respecta el bloc no reasignable

# Funcions = son accions que retornen valors
```js
function sumaliDos (param1) {
    return 2 + param1
}

a = (param1) => {return 2 + param1}

a = (param1) => 2 + param1

```

# operadors logics = comparadors

=== estrictament igual (respecta el tipus)
== lliurament igual (no respecta el tipus)
!== negacio estricta
!= negacio lliure
< mes gran
> mes petit
>= mes gran o igual
<= mes peti o igual
!variable negació
!!variable doble negació (passara booleà)

# Array.prototip
map -> itera pels elements. torna un array
llista.map(item => !!item)

forEach -> itera pels elements. no torna valor

some -> itera retornan true si algun dels elements es true

every -> itera retarna true si tos son true
reduce -> acumula els items fins retorna un element
llista.reduce((prev, item) => ({...prev, [item]: !!item }), {})