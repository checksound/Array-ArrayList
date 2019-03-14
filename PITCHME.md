# Array & Array List
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
---?gist=MassimoCappellano/f635ef66e0a4ec1b156a392cccf923ed&lang=Java&title=Dinamic array of people

Le tre classi che hanno il comportamento di un array dinamico sono molto simili come si può notare.

---
### Tipi Parametrici

Vediamo che la logica di base non cambia molto, per questo sono stati definiti i tipi parametrici, tipi che sono customizzati in base al tipo contenuto. Vederemo nelle prossime lezioni di trattare l'argomento.

---?gist=MassimoCappellano/489a4111f3a941e2c7ba4daa552ab520&lang=Java&title=Dinamic Array generico

Solo esempio introduttivo... vederemo in seguito
---?gist=MassimoCappellano/1007e91a902fe452cb18f271ef8abf7d&lang=Java&title=Esempio con DinamicArrayGeneric

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

@snap[span-100]
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

Gli ultimi due metodi `list.remove(obj)` e `list.indexOf(obj)` utilizzano `obj.equals(Object o)` per trovare l'oggetto da rimuovere o la posizione dell'oggetto nella lista.

E' importante che quindi il metodo `equals` sia reimplementato secondo la logica di confronto per noi opportuna.

---?gist=MassimoCappellano/f4bc46f00f82a9c361e4fe23bf1f70bd&lang=Java&title=Esempio con ArrayList

---
Abbiamo visto come, da tipo array, si possono costruire array dinamici. La classe del JDK `java.util.ArrayList` ha il comportamento degli array dinamici ed è implementata internamente, come dice il nome, con un array che contiene gli elementi.

La classe `ArrayList` implementa l'interfaccia `java.util.List`.

Anche la classe `java.util.LinkedList` implementa l'interfaccia `java.util.List`.
---
@img[shadow](assets/img/ArrayListVsLinkedList.png)

---
Le differenze tra `ArrayList` e `LinkedList` dipendono dalla struttura dati interna utilizzata: un array nel caso di `ArrayList` mentre, nel caso della `LinkedList`, è utillizzata una lista dinamica. I metodi che espongono sono uguali perchè ambedue implementano l'intarfaccia `java.util.List`.

Vediamo cos'è una lista dinamica.








