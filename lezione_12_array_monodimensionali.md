# Array monodimensionali

Gli array monodimensionali sono una struttura dati fondamentale nella programmazione, in grado di contenere una sequenza di elementi dello stesso tipo. In questo articolo approfondiremo la dichiarazione, l'inizializzazione e l'accesso agli elementi di un array monodimensionale.

## Dichiarazione

La dichiarazione di un array monodimensionale avviene specificando il tipo degli elementi contenuti nell'array e la dimensione dell'array stessa. Ad esempio, per dichiarare un array di interi di dimensione 5, si utilizza la seguente sintassi:

```c
int array[5];
```

## Inizializzazione

L'inizializzazione di un array monodimensionale consiste nell'assegnare dei valori iniziali agli elementi dell'array. Questo può avvenire durante la dichiarazione dell'array o successivamente, utilizzando un ciclo o assegnando valori singoli agli elementi. Ad esempio, per inizializzare un array di interi con valori predefiniti, si può utilizzare la seguente sintassi:

```c
int array[5] = {1, 2, 3, 4, 5};
```

## Accesso agli elementi

Per accedere agli elementi di un array monodimensionale è necessario utilizzare l'indice dell'elemento desiderato. Gli indici degli elementi in un array monodimensionale partono da 0 fino alla dimensione dell'array meno uno. Ad esempio, per accedere al terzo elemento di un array si utilizza la seguente sintassi:

```c
int terzo_elemento = array[2];
```

È importante prestare attenzione al fatto che l'accesso a un elemento al di fuori dei limiti dell'array può causare comportamenti indesiderati o errori nel programma.

In conclusione, gli array monodimensionali sono una struttura dati essenziale nella programmazione, utilizzata per memorizzare una sequenza di elementi dello stesso tipo. Conoscere come dichiarare, inizializzare e accedere agli elementi di un array monodimensionale è fondamentale per scrivere codice efficiente e corretto.