# Passaggio parametri

Il passaggio dei parametri è un concetto fondamentale nella programmazione e può avvenire in due modi principali: per valore e per riferimento. In questo articolo esamineremo le differenze tra i due metodi e le implicazioni pratiche che possono derivarne.

## Passaggio per valore

Nel passaggio per valore, una copia del valore del parametro viene passata alla funzione chiamata. Questo significa che qualsiasi modifica apportata al parametro all'interno della funzione non avrà effetto sulla variabile originale passata alla funzione.

```python
def incrementa_numero(numero):
    numero += 1

x = 5
incrementa_numero(x)
print(x)  # Output: 5
```

Nell'esempio sopra, la funzione `incrementa_numero` incrementa il valore del parametro `numero` di 1, ma poiché viene passato per valore, la variabile `x` rimane invariata.

## Passaggio per riferimento

Nel passaggio per riferimento, invece, viene passato il riferimento alla variabile stessa, piuttosto che una copia del suo valore. Questo significa che qualsiasi modifica apportata al parametro all'interno della funzione si rifletterà anche sulla variabile originale.

```python
def incrementa_lista(lista):
    lista.append(4)

my_list = [1, 2, 3]
incrementa_lista(my_list)
print(my_list)  # Output: [1, 2, 3, 4]
```

Nell'esempio sopra, la funzione `incrementa_lista` aggiunge l'elemento 4 alla lista passata come parametro. Poiché viene passata per riferimento, la modifica si riflette sulla variabile `my_list` originale.

## Conclusioni

È importante comprendere la differenza tra passaggio per valore e per riferimento per evitare comportamenti inaspettati nei programmi. In generale, il passaggio per valore è più sicuro e prevedibile, mentre il passaggio per riferimento può portare a effetti collaterali indesiderati. La scelta del metodo dipende dalle esigenze specifiche del programma e dalla gestione dei dati.