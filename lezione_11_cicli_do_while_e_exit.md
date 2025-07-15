# Cicli: do while e exit

I cicli sono una struttura fondamentale della programmazione che permette di ripetere un blocco di istruzioni un certo numero di volte o fino a quando una determinata condizione risulta vera. Tra i cicli più comuni troviamo il ciclo `while`, che ripete un blocco di istruzioni finché una condizione è vera, e il ciclo `do while`, che invece esegue almeno una volta il blocco di istruzioni prima di valutare la condizione.

Il ciclo `do while` è molto utile quando si vuole garantire che un blocco di istruzioni venga eseguito almeno una volta, anche se la condizione di uscita è già vera all'inizio. Ad esempio:

```java
int numero = 5;
do {
    System.out.println(numero);
    numero--;
} while (numero > 0);
```

In questo esempio, il blocco di istruzioni viene eseguito almeno una volta, stampando il valore di `numero` e decrementandolo fino a quando non diventa minore o uguale a 0.

Spesso può essere necessario interrompere un ciclo in anticipo, anziché aspettare che la condizione di uscita diventi vera. In tal caso, si può utilizzare l'istruzione `exit`, che permette di uscire immediatamente da un ciclo. Ad esempio:

```java
int numero = 1;
while (numero < 10) {
    if (numero == 5) {
        System.out.println("Uscita anticipata");
        break;
    }
    System.out.println(numero);
    numero++;
}
```

In questo caso, il ciclo `while` viene interrotto anticipatamente quando `numero` raggiunge il valore 5, stampando il messaggio "Uscita anticipata" e uscendo dal ciclo.

In conclusione, i cicli `do while` e l'istruzione `exit` sono strumenti utili per gestire la ripetizione condizionata e l'interruzione anticipata all'interno di un programma. Utilizzarli in modo appropriato può rendere il codice più chiaro e efficiente, migliorando la leggibilità e la manutenibilità del software.