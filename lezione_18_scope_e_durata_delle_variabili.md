# Scope e durata delle variabili

Le variabili sono elementi fondamentali all'interno di un programma, in quanto consentono di memorizzare e manipolare i dati necessari per l'esecuzione delle operazioni previste. È importante comprendere la differenza tra lo scope e la durata delle variabili al fine di garantire un corretto funzionamento del programma e ottimizzare l'utilizzo delle risorse disponibili.

## Scope delle variabili

Lo scope di una variabile definisce la porzione di codice in cui la variabile stessa è accessibile e può essere utilizzata. Le variabili possono essere dichiarate con diversi livelli di scope, tra cui locale, globale, save e common blocks.

- **Variabili locali**: sono definite all'interno di una specifica funzione o subroutine e sono accessibili solo all'interno di essa. Una volta che la funzione termina, le variabili locali vengono distrutte e il loro valore non è più accessibile.
  
- **Variabili globali**: sono definite al di fuori di qualsiasi funzione o subroutine e sono accessibili da qualsiasi parte del programma. Le variabili globali mantengono il loro valore anche al di fuori del blocco di codice in cui sono state dichiarate.
  
- **Variabili save**: sono simili alle variabili locali, ma mantengono il loro valore anche dopo che la funzione o subroutine in cui sono state dichiarate è terminata. Le variabili save mantengono il loro valore fino alla fine dell'esecuzione del programma.
  
- **Common blocks**: sono aree di memoria condivise tra diverse parti del programma e consentono di condividere dati tra variabili diverse. Le variabili all'interno di un common block mantengono il loro valore anche al di fuori del blocco di codice in cui sono state dichiarate.

## Durata delle variabili

La durata di una variabile indica per quanto tempo la variabile esiste all'interno del programma e per quanto tempo il suo valore è accessibile. Le variabili possono avere durata statica o dinamica.

- **Variabili a durata statica**: sono allocate una sola volta durante l'esecuzione del programma e mantengono il loro valore per l'intera durata dell'esecuzione del programma. Le variabili statiche vengono allocate all'inizio dell'esecuzione del programma e deallocare alla sua conclusione.
  
- **Variabili a durata dinamica**: vengono allocate e deallocate dinamicamente durante l'esecuzione del programma. Le variabili dinamiche mantengono il loro valore solo per il tempo in cui sono allocate e vengono deallocate quando non sono più necessarie.

È importante definire correttamente lo scope e la durata delle variabili all'interno di un programma al fine di garantire un utilizzo efficiente delle risorse e evitare errori di esecuzione. Utilizzare le variabili in modo oculato contribuisce a migliorare la leggibilità e la manutenibilità del codice, facilitando la risoluzione di eventuali problemi e il debugging del programma.