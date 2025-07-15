# Input e output su file

Quando si lavora con la programmazione, è spesso necessario leggere e scrivere dati da e su file. Questa operazione è fondamentale per salvare informazioni in modo permanente e per poterle utilizzare in momenti successivi.

## Lettura da file

Per leggere dati da un file in un programma, è necessario aprire il file in modalità lettura e utilizzare una variabile per memorizzare i dati letti. Ad esempio, possiamo utilizzare il seguente codice in Python per leggere il contenuto di un file di testo:

```python
with open('file.txt', 'r') as file:
    data = file.read()
    print(data)
```

In questo caso, il file viene aperto in modalità lettura ('r') e il suo contenuto viene letto e memorizzato nella variabile `data`. Infine, il contenuto del file viene stampato a schermo.

## Scrittura su file

Analogamente, per scrivere dati su un file, è necessario aprire il file in modalità scrittura e utilizzare il metodo `write()` per scrivere i dati. Ad esempio, possiamo utilizzare il seguente codice in Python per scrivere una stringa su un file di testo:

```python
data = 'Questo è un esempio di testo da scrivere su file.'
with open('output.txt', 'w') as file:
    file.write(data)
```

In questo caso, il file viene aperto in modalità scrittura ('w') e la stringa `data` viene scritta sul file. È importante notare che la modalità scrittura sovrascrive il contenuto del file esistente, quindi è necessario fare attenzione a non perdere dati importanti.

## Conclusioni

L'input e l'output su file sono operazioni comuni nella programmazione e sono fondamentali per gestire in modo efficiente i dati. È importante conoscere le modalità di apertura dei file e i metodi per leggere e scrivere dati in modo corretto. Con le giuste conoscenze e pratiche, è possibile manipolare i file in modo sicuro ed efficace.