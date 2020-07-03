# Paralelizacao-BucketOpenMP
Este repositório contém o projeto final da ACIEPE(Atividade Curricular de Integração entre Ensino, Pesquisa e Extensão) - "Programação paralela:
das threads aos FPGAs - uma introdução ao tema", ofertada pelo Departamento de Computação da UFSCar - São Carlos.

O projeto final é um artigo sobre a paralelização do algoritmo de ordenação Bucket Sort com a API Open Multi-Processing (OpenMP), no qual foi comparado o desempenho da versão sequencial e da versão paralela.

A versão inicial do código Bucket Sort foi retirada do site [Programiz](https://www.programiz.com/ "Programiz") e pode ser encontrado [aqui](https://www.programiz.com/dsa/bucket-sort "aqui"). 

Os testes de desempenho foram realizados no [Coliru](https://coliru.stacked-crooked.com/ "Coliru") onde eles podem ser compilados e executados usando o comando:
`g++ -std=c++17 -O2 -Wall -fopenmp -pedantic main.cpp && time ./a.out`
