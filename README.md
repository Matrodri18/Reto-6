# Reto-6
## 1. Imprimir un listado con los numeros del 1 al 100, cada uno con su respectivo cuadrado.

```mermaid
flowchart TD
    A(Inicio) -->B[n = 0] 
    B --> C{n <= 100}
    C -->|SÍ|D["print (n, : , n ** 2)" ]
    D -->E[n = n + 1]
    E -->C
    C -->|NO|F
F(Fin)
```
## 2. Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
#### Numeros Impares
```mermaid
flowchart TD
    A(Inicio) --> B[n=1]
    B --> C[n<1000]
    C --> |Sí n%2 != 0|D["print n"]
    D --> E["n=n+1"]
    E --> C
    C --> |Sí n%2 == 0|E 
    C --> |No|F[Fin]
```
#### Numeros Pares
```mermaid
flowchart TD
    A(Inicio) --> B[n=2]
    B --> C[n<=1000]
    C --> |Sí n%2==0|D["Print n"]
    D --> E["n=n+1"]
    E --> C
    C--> |Sí n%2!=0|E
    C -->|No|F[Fin]
```
## 3. Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n>=2 dado.
```mermaid
flowchart TD
    A(Inicio) --> B[n]
    B --> C[2<=n]
    C --> |Sí n%2==0|D["Print n"]
    D --> E["n=n-1"]
    E --> C
    C --> |Sí n%2!=0|G["Print n-1"]
    G --> C
    E -->|Sí n-1<2|F[Fin]
```

