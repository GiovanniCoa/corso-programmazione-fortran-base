# Struttura di un programma Fortran

Il linguaggio di programmazione Fortran è ampiamente utilizzato nel campo della computazione scientifica e ingegneristica per la sua potenza e versatilità. La struttura di un programma Fortran segue uno schema ben definito, composto da un programma principale, dichiarazioni e il corpo del programma.

## Programma principale

Il programma principale in un programma Fortran è identificato dal blocco `PROGRAM` seguito dal nome del programma. Ad esempio:

```fortran
PROGRAM main_program
```

Il programma principale è il punto di partenza dell'esecuzione del programma e può contenere chiamate a procedure esterne e altri moduli.

## Dichiarazioni

Le dichiarazioni in un programma Fortran sono utilizzate per definire le variabili, costanti e tipi di dati utilizzati nel programma. Le dichiarazioni vengono solitamente posizionate all'inizio del programma e possono includere dichiarazioni di variabili, costanti e tipi di dati. Ad esempio:

```fortran
INTEGER :: a, b
REAL :: x, y
PARAMETER (pi = 3.14159)
```

Le dichiarazioni sono utilizzate per definire le variabili e costanti necessarie per l'esecuzione del programma e per garantire la corretta allocazione di memoria.

## Corpo del programma

Il corpo del programma Fortran contiene le istruzioni e le operazioni che vengono eseguite durante l'esecuzione del programma. Le istruzioni nel corpo del programma sono eseguite sequenzialmente e possono includere operazioni matematiche, condizionali e cicli. Ad esempio:

```fortran
a = 10
b = 20
x = a + b
y = sin(x)
```

Il corpo del programma contiene le istruzioni necessarie per eseguire le operazioni richieste e produrre l'output desiderato.

In conclusione, la struttura di un programma Fortran è composta da un programma principale, dichiarazioni e il corpo del programma. Seguendo questo schema, è possibile scrivere programmi efficaci e efficienti per risolvere una vasta gamma di problemi computazionali.