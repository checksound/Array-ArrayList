# Array & Arraly List
---

## DINAMIC ARRAY
Implementiamo un array dinamico da un array base. In questo caso un arrray di `int`.

---?gist=MassimoCappellano/14094c0aabca84f4f2eb9e24a81fb496&lang=Java&title=Dinamic Array of ints

@[1-9](attributi private `items` e `itemCt`)
@[10-35](get item, set item e size())
@[36-58](add item e remove item)

---
Se avessi avuto bisogno di un array dinamico di `String`?

---?gist=MassimoCappellano/0d4dad68bf46818770793bc2576e2afb&lang=Java&title=Dinamic array of strings

@[1-9](attributi private `items` e `itemCt`)
@[10-35](get item, set item e size())
@[36-58](add item e remove item)

---
E un array dinamico di una mia classe ad esempio `Persona`? 
---
Vediamo che la logica di base non cambia molto, per queste sono stati definiti i tipi parametrici, tipi che sono customizzati in base al tipo contenuto. Vederemo nelle prossime lezioni di trattare l'argomento.
---

#### Utilizzo della classe `ArrayList`

`java.util.ArrayList` è una delle classi standard del JDK, fa parte del Java Collection Framework.

E' un tipo parametrico `java.util.ArrayList<T>`. 

```java
ArrayList<String> namelist = new ArrayList<String>();

ArrayList<Player> playerList = new ArrayList<Player>();
```
---
@snap[north-west]
#### Metodi
@snapend

@snap[west span-95]
@ul[spaced text-red]
- list.size()
- list.add(obj)
- list.get(N) , lancia ArrayIndexOutOfBoundException se N >= list.size()
- list.set(N, obj)
- list.clear()
- list.remove(N)
- list.remove(obj)
- list.indexOf(obj)
@ulend
@snapend
---

## Programmare con ArrayList

