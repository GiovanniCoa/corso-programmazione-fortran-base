# Allocazione dinamica della memoria

L'allocazione dinamica della memoria è un concetto fondamentale nella programmazione moderna, che consente di gestire in modo efficiente la memoria disponibile durante l'esecuzione di un programma. In particolare, l'uso di allocatable e deallocatable è una tecnica avanzata che consente di assegnare e liberare memoria in modo dinamico, in base alle esigenze del programma.

## Cos'è l'allocazione dinamica della memoria

L'allocazione dinamica della memoria è un processo attraverso il quale un programma assegna e libera memoria durante l'esecuzione. Questo è in contrasto con l'allocazione statica, in cui la memoria viene riservata in fase di compilazione e non può essere modificata durante l'esecuzione del programma. L'allocazione dinamica consente ai programmi di gestire in modo efficiente la memoria disponibile, evitando sprechi e consentendo di adattarsi alle esigenze specifiche del programma.

## Utilizzo di allocatable e deallocatable

In Fortran, è possibile utilizzare le dichiarazioni `allocatable` e `deallocatable` per gestire l'allocazione dinamica della memoria. Le variabili dichiarate come `allocatable` possono essere assegnate a una determinata dimensione solo durante l'esecuzione del programma, consentendo di riservare la quantità di memoria necessaria in base alle esigenze specifiche del programma. Una volta che la memoria non è più necessaria, è possibile deallocarla utilizzando la dichiarazione `deallocatable`, liberando così la memoria precedentemente riservata.

Ecco un esempio di come utilizzare `allocatable` e `deallocatable` in Fortran:

```fortran
program allocazione_memoria
    real, allocatable :: array(:)

    allocate(array(100)) ! Allocazione di un array di dimensione 100

    ! Utilizzo dell'array

    deallocate(array) ! Deallocazione della memoria
end program allocazione_memoria
```

In questo esempio, viene allocata una memoria per un array di dimensione 100, utilizzata e infine deallocata una volta che non è più necessaria. Questo permette di gestire in modo efficiente la memoria disponibile durante l'esecuzione del programma, evitando sprechi e ottimizzando le prestazioni.

## Conclusioni

L'allocazione dinamica della memoria, tramite l'uso di `allocatable` e `deallocatable`, è una tecnica avanzata che consente di gestire in modo efficiente la memoria disponibile durante l'esecuzione di un programma. Questo permette ai programmatori di adattare le risorse disponibili alle esigenze specifiche del programma, ottimizzando le prestazioni e evitando sprechi. È importante comprendere i principi di base dell'allocazione dinamica della memoria per scrivere programmi efficienti e affidabili.