# Common blocks e moduli

Nella programmazione in Fortran, i common blocks e i moduli sono due strumenti utilizzati per la condivisione di dati tra procedure. Questi due meccanismi sono fondamentali per garantire la coerenza e l'accessibilità dei dati all'interno di un programma.

## Common blocks

I common blocks sono aree di memoria condivise tra le diverse unità di programma. Questo significa che le variabili definite all'interno di un common block possono essere utilizzate da più procedure all'interno del programma. Per definire un common block, è necessario utilizzare la seguente sintassi:

```
COMMON /nome_comune/ lista_variabili
```

Le variabili definite all'interno del common block devono essere dichiarate come comuni in tutte le procedure che le utilizzano. Inoltre, è importante specificare la dimensione delle variabili nel common block per garantire la corretta allocazione di memoria.

## Moduli

I moduli sono un'altra forma di condivisione di dati tra le procedure in Fortran. Un modulo è un'unità di programma che contiene dichiarazioni di variabili, costanti, tipi di dati e procedure. Per utilizzare un modulo in un programma, è necessario utilizzare la seguente sintassi:

```
USE nome_modulo
```

Una volta dichiarato l'utilizzo di un modulo, è possibile accedere a tutte le variabili e procedure definite all'interno di esso. I moduli offrono un maggiore controllo sulla visibilità delle variabili e delle procedure, evitando potenziali conflitti di nomi tra le diverse unità di programma.

## Conclusione

In conclusione, i common blocks e i moduli sono due strumenti fondamentali per la condivisione di dati tra le diverse procedure in Fortran. I common blocks permettono la condivisione di variabili all'interno di un programma, mentre i moduli offrono un maggiore controllo sulla visibilità e l'accessibilità dei dati. È importante utilizzare correttamente entrambi i meccanismi per garantire la coerenza e l'efficienza del programma.