# Reto_3

´´´ mermaid 
flowchart TD
    n1["INICIO"] --> n2["número n"]
    n2 --> n3["Lista de 2 hasta n+1"]
    n3 --> n4["i = 2"]
    n4 --> n5["¿El residuo de la división de n/i es igual a cero?"]
    n5 -- SI --> n6["i = j"]
    n5 -- NO --> n7["¿Es i menor a n?"]
    n6 --> n9["¿j es menor a n+1?"]
    n9 -- SI --> n10["Descartar número igual a j de la lista"]
    n10 --> n12["Se suma j + i, para que sea multiplo de i"]
    n12 --> n9 & n7
    n7 -- NO --> n13["FIN"]
    n7 -- SI --> n5
    n1@{ shape: rounded}
    n2@{ shape: lean-l}
    n5@{ shape: diam}
    n7@{ shape: diam}
    n9@{ shape: diam}
    n13@{ shape: rounded}
´´´
