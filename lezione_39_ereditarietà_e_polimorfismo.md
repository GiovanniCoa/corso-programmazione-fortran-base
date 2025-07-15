# Ereditarietà e polimorfismo in Fortran

L'ereditarietà e il polimorfismo sono concetti fondamentali della programmazione orientata agli oggetti (OOP) che permettono di creare gerarchie di classi e di scrivere codice più flessibile e riutilizzabile. In Fortran, un linguaggio noto per la sua potenza nel calcolo scientifico, è possibile implementare questi concetti in modo efficiente e avanzato.

## Ereditarietà

L'ereditarietà consente di definire una nuova classe basandosi su una classe esistente, ereditandone i metodi e gli attributi. In Fortran, è possibile implementare l'ereditarietà utilizzando il costrutto `extends` all'interno della dichiarazione di una classe. Ad esempio:

```fortran
module Animal
  type :: Animal
    integer :: legs
  end type Animal
end module Animal

module Dog
  use Animal
  type, extends(Animal) :: Dog
    character(len=20) :: breed
  end type Dog
end module Dog
```

Nell'esempio sopra, la classe `Dog` eredita l'attributo `legs` dalla classe `Animal` e aggiunge un nuovo attributo `breed`. In questo modo è possibile creare una gerarchia di classi per modellare concetti complessi in modo più strutturato.

## Polimorfismo

Il polimorfismo permette di trattare oggetti di classi diverse in modo uniforme, chiamando un metodo comune che si comporta in modo diverso a seconda della classe dell'oggetto su cui viene chiamato. In Fortran, è possibile implementare il polimorfismo utilizzando procedure di tipo `abstract` e procedure di tipo `deferred`. Ad esempio:

```fortran
module Animal
  type, abstract :: Animal
    integer :: legs
    procedure(Describe), deferred :: Describe
  contains
    procedure :: GetLegs
end module Animal

module Dog
  use Animal
  type, extends(Animal) :: Dog
    character(len=20) :: breed
  contains
    procedure :: Describe => DescribeDog
end module Dog

abstract interface
  subroutine Describe(obj)
    import :: Animal
    class(Animal), intent(in) :: obj
  end subroutine Describe
end interface

subroutine DescribeDog(obj)
  class(Dog), intent(in) :: obj
  print *, 'This is a ', obj%breed, ' dog with ', obj%legs, ' legs'
end subroutine DescribeDog
```

Nell'esempio sopra, la classe `Animal` definisce un metodo `Describe` di tipo `deferred`, che deve essere implementato dalle classi che ereditano da `Animal`. La classe `Dog` implementa il metodo `Describe` in modo specifico per il cane, permettendo di chiamare il metodo `Describe` su un oggetto di tipo `Dog` in modo polimorfico.

In conclusione, l'ereditarietà e il polimorfismo sono concetti avanzati della programmazione orientata agli oggetti che possono essere implementati in modo efficiente e potente in Fortran. Utilizzando questi concetti è possibile creare codice più flessibile, riutilizzabile e strutturato, facilitando lo sviluppo di software complesso