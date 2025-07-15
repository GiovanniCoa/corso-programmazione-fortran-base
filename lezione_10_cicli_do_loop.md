# Cicli: do loop

Il `do loop` è una struttura di controllo che permette di eseguire ripetutamente un blocco di istruzioni finché non viene verificata una condizione di uscita. Questo tipo di ciclo è particolarmente utile quando si conosce il numero esatto di iterazioni da eseguire.

## Sintassi del do loop

La sintassi del `do loop` in molti linguaggi di programmazione è la seguente:

```
do {
    // blocco di istruzioni da ripetere
} while (condizione);
```

In questo caso, il blocco di istruzioni verrà eseguito almeno una volta, prima di verificare la condizione di uscita. Se la condizione è falsa, il ciclo termina e il controllo passa alla successiva istruzione dopo il `do loop`.

## Esempio pratico

Supponiamo di voler stampare i numeri da 1 a 10 utilizzando un `do loop` in linguaggio C:

```c
#include <stdio.h>

int main() {
    int i = 1;

    do {
        printf("%d\n", i);
        i++;
    } while (i <= 10);

    return 0;
}
```

In questo caso, il programma stamperà i numeri da 1 a 10, incrementando di volta in volta la variabile `i` finché non raggiunge il valore 10.

## Conclusioni

Il `do loop` è una struttura di controllo fondamentale nella programmazione, che permette di eseguire ripetutamente un blocco di istruzioni finché non viene soddisfatta una condizione di uscita. È particolarmente utile quando si conosce il numero esatto di iterazioni da eseguire, garantendo l'esecuzione del blocco almeno una volta.