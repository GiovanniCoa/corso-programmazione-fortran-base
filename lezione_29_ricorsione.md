# Ricorsione

La ricorsione è un concetto fondamentale nella programmazione che si basa sull'idea di una funzione o subroutine che si chiama se stessa. Questo approccio permette di risolvere problemi complessi suddividendoli in sottoproblemi più semplici, creando così una struttura a catena che si sviluppa fino alla soluzione finale.

## Funzioni ricorsive

Le funzioni ricorsive sono definite da un'invocazione della funzione stessa all'interno del suo corpo. Questo meccanismo consente di ripetere l'esecuzione di un blocco di istruzioni fino a quando non viene soddisfatta una condizione di terminazione. Ad esempio, la funzione fattoriale può essere implementata in modo ricorsivo nel seguente modo:

```python
def fattoriale(n):
    if n == 0:
        return 1
    else:
        return n * fattoriale(n-1)
```

In questo caso, la funzione `fattoriale` si chiama ricorsivamente fino a quando `n` non diventa uguale a 0, momento in cui viene restituito il valore 1.

## Subroutine ricorsive

Anche le subroutine possono essere implementate in modo ricorsivo, consentendo di risolvere problemi complessi attraverso una struttura gerarchica. Ad esempio, un algoritmo di ordinamento come il quicksort può essere implementato in modo ricorsivo:

```python
def quicksort(arr):
    if len(arr) <= 1:
        return arr
    else:
        pivot = arr[0]
        less = [x for x in arr[1:] if x <= pivot]
        greater = [x for x in arr[1:] if x > pivot]
        return quicksort(less) + [pivot] + quicksort(greater)
```

In questo caso, la subroutine `quicksort` si chiama ricorsivamente per ordinare le parti "minor" e "maggiore" dell'array di input.

## Conclusioni

La ricorsione è un potente strumento che consente di risolvere problemi complessi in modo elegante e efficiente. Tuttavia, è importante prestare attenzione alla gestione della memoria e alla definizione corretta delle condizioni di terminazione per evitare loop infiniti. Con una corretta progettazione e implementazione, la ricorsione può essere uno strumento prezioso per affrontare sfide di programmazione di varia complessità.