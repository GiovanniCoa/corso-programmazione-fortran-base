# Programmazione orientata agli oggetti in Fortran

La programmazione orientata agli oggetti (OOP) è un paradigma di programmazione che si basa sulla creazione di oggetti che contengono dati e metodi per manipolare questi dati. Fortran, un linguaggio di programmazione ad alto livello utilizzato principalmente per il calcolo scientifico e l'elaborazione numerica, ha introdotto il supporto per la programmazione orientata agli oggetti a partire dalla versione Fortran 2003.

## Concetti base della programmazione orientata agli oggetti

I concetti chiave della programmazione orientata agli oggetti includono l'incapsulamento, l'ereditarietà e il polimorfismo. 
- **Incapsulamento**: è il concetto che permette di nascondere l'implementazione interna di un oggetto e di esporre solo le sue interfacce pubbliche.
- **Ereditarietà**: permette la creazione di nuove classi che ereditano le caratteristiche e i comportamenti di una classe esistente.
- **Polimorfismo**: permette a oggetti di classi diverse di rispondere allo stesso messaggio in modi diversi.

## Sintassi della programmazione orientata agli oggetti in Fortran

Per definire una classe in Fortran, si utilizza il costrutto `type`, che permette di dichiarare un tipo di dato complesso contenente sia dati che metodi. Ad esempio:

```fortran
module mod_mia_classe
  type :: mia_classe
    integer :: attributo
    contains
    procedure :: metodo1
  end type mia_classe

contains

subroutine mia_classe::metodo1()
  ! implementazione del metodo1
end subroutine metodo1

end module mod_mia_classe
```

Per creare un oggetto di una classe, si utilizza la seguente sintassi:

```fortran
use mod_mia_classe
type(mia_classe) :: oggetto
```

Per accedere agli attributi e ai metodi di un oggetto, si utilizza l'operatore `%`. Ad esempio:

```fortran
oggetto%attributo = 10
call oggetto%metodo1()
```

## Conclusioni

La programmazione orientata agli oggetti in Fortran offre agli sviluppatori la possibilità di scrivere codice più modulare, riutilizzabile e manutenibile. Utilizzando i concetti di incapsulamento, ereditarietà e polimorfismo, è possibile creare gerarchie di classi e oggetti che riflettono in modo più accurato la struttura del problema da risolvere. Sebbene Fortran sia principalmente noto per la sua programmazione procedurale, l'aggiunta del supporto per la programmazione orientata agli oggetti ha reso il linguaggio più flessibile e potente per una vasta gamma di applicazioni.