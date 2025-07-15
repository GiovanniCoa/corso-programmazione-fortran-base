# Introduzione a MPI

MPI (Message Passing Interface) è uno standard di comunicazione utilizzato per la programmazione parallela distribuita su sistemi con architettura a memoria distribuita. Questo standard fornisce un insieme di funzioni e metodi per consentire ai processi di comunicare tra loro in modo efficiente e sincronizzato.

## Concetti base di MPI

### Comunicazione punto a punto

Una delle caratteristiche principali di MPI è la capacità di consentire la comunicazione tra i processi in modo diretto, utilizzando messaggi di dimensioni variabili. Questo approccio permette una maggiore flessibilità nella progettazione e implementazione di algoritmi paralleli.

### Comunicazione collettiva

MPI supporta anche operazioni di comunicazione collettiva che coinvolgono più processi contemporaneamente. Queste operazioni possono essere utilizzate per implementare algoritmi paralleli più complessi, come la riduzione, la scansione e lo scatter.

### Topologie MPI

MPI consente anche di definire topologie di comunicazione tra i processi, ad esempio topologie a griglia, a anello o a albero. Questo permette di ottimizzare ulteriormente le comunicazioni tra i processi e migliorare le prestazioni complessive del sistema parallelo.

## Esempio di codice MPI

Di seguito è riportato un esempio semplice di codice in MPI che mostra come due processi possono scambiarsi dei messaggi utilizzando le funzioni di comunicazione punto a punto:

```markdown
#include <stdio.h>
#include <mpi.h>

int main(int argc, char** argv) {
    int rank, size, msg;
    MPI_Init(&argc, &argv);
    MPI_Comm_rank(MPI_COMM_WORLD, &rank);
    MPI_Comm_size(MPI_COMM_WORLD, &size);

    if (rank == 0) {
        msg = 42;
        MPI_Send(&msg, 1, MPI_INT, 1, 0, MPI_COMM_WORLD);
    } else if (rank == 1) {
        MPI_Recv(&msg, 1, MPI_INT, 0, 0, MPI_COMM_WORLD, MPI_STATUS_IGNORE);
        printf("Process 1 received message: %d\n", msg);
    }

    MPI_Finalize();
    return 0;
}
```

Questo codice crea due processi, uno dei quali invia un messaggio all'altro tramite la funzione `MPI_Send`, mentre l'altro riceve il messaggio tramite la funzione `MPI_Recv`.

## Conclusioni

MPI è uno strumento potente e flessibile per la programmazione parallela distribuita, che consente di realizzare algoritmi paralleli efficienti e scalabili su sistemi con architettura a memoria distribuita. Con una corretta progettazione e implementazione, è possibile sfruttare appieno le potenzialità di MPI per ottenere prestazioni ottimali nei calcoli paralleli.