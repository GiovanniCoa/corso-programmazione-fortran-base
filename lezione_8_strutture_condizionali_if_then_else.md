# Strutture condizionali: if then else

Le strutture condizionali sono uno strumento fondamentale nella programmazione per controllare il flusso del programma in base a determinate condizioni. Uno dei costrutti più comuni è l'istruzione "if then else", che permette di eseguire un blocco di codice se una condizione è vera e un altro blocco se la condizione è falsa.

## Sintassi

La sintassi dell'istruzione "if then else" è la seguente:

```python
if condizione:
    # blocco di codice da eseguire se la condizione è vera
else:
    # blocco di codice da eseguire se la condizione è falsa
```

## Esempio

Ecco un esempio di utilizzo dell'istruzione "if then else" in Python:

```python
x = 10

if x > 5:
    print("x è maggiore di 5")
else:
    print("x è minore o uguale a 5")
```

In questo caso, se il valore di x è maggiore di 5, verrà stampato il messaggio "x è maggiore di 5", altrimenti verrà stampato il messaggio "x è minore o uguale a 5".

## Condizioni nidificate

Le condizioni possono essere anche nidificate, cioè all'interno di un blocco condizionale è possibile inserire un altro blocco condizionale. Ad esempio:

```python
x = 10
y = 20

if x > 5:
    if y > 15:
        print("Entrambi x e y sono maggiori di 5 e 15 rispettivamente")
    else:
        print("x è maggiore di 5 ma y è minore o uguale a 15")
else:
    print("x è minore o uguale a 5")
```

In questo caso, vengono valutate due condizioni: se x è maggiore di 5 e se y è maggiore di 15.

Le strutture condizionali sono uno strumento potente per controllare il flusso del programma in base a determinate condizioni e permettono di scrivere codice più flessibile e adattabile a diverse situazioni.