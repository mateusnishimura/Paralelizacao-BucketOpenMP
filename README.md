# Paralelizacao-BucketOpenMP
Este repositório contém o projeto final da ACIEPE(Atividade Curricular de Integração entre Ensino, Pesquisa e Extensão) - "Programação paralela:
das threads aos FPGAs - uma introdução ao tema", ofertada pelo Departamento de Computação da UFSCar - São Carlos.

O projeto final é um artigo sobre a paralelização do algoritmo de ordenação Bucket Sort com a API Open Multi-Processing (OpenMP), no qual foi comparado o desempenho da versão sequencial e da versão paralela.

A versão inicial do código Bucket Sort foi retirada do site [Programiz](https://www.programiz.com/ "Programiz") e pode ser encontrado [aqui](https://www.programiz.com/dsa/bucket-sort "aqui"). 

Os testes de desempenho foram realizados no [Coliru](https://coliru.stacked-crooked.com/ "Coliru") onde eles podem ser compilados e executados usando o comando:
`g++ -std=c++17 -O2 -Wall -fopenmp -pedantic main.cpp && time ./a.out`

A tabela a seguir demonstra o desempenho da versão sequencial e versão paralela comparados. Os números linkados redirecionam para o site Coliru que mostram os testes realizados e também possibilitam a execução ou edição do código.

|  Nº de elementos | Nº baldes  | Intervalo | Versão Sequencial  | Versão  Paralela  |
| :------------: | :------------: | :------------: | :------------: | :------------: |
| 100  | 100  | 100  | [0.010s](https://coliru.stacked-crooked.com/a/9b2b0b8d7a52ce79 "0.010s")  | [0.09s](https://coliru.stacked-crooked.com/a/93490aa04f06d355 "0.09s")  |
|  1.000 | 100  |  100 | [0.011s](https://coliru.stacked-crooked.com/a/fe7902d222242648 "0.011s")  | [0.012s](https://coliru.stacked-crooked.com/a/06ae6c8c40db3f4c "0.012s")  |
| 10.000  | 100  | 100 | [0.768s](https://coliru.stacked-crooked.com/a/c145932c8ff310b1 "0.768s")  | [0.020s](https://coliru.stacked-crooked.com/a/bc46a1d3a0eab0f6 "0.020s")  |
| 100.000  | 1.000 | 1.000  | [2.754s](https://coliru.stacked-crooked.com/a/be9b0057592d7831 "2.754s")  | [2.608s](https://coliru.stacked-crooked.com/a/b49f03c9817f431c "2.608s")|
| 100.000  | 10.000  | 1.000  | [2.746s](https://coliru.stacked-crooked.com/a/4432ee99c7b04237 "2.746s")  | [2.689s](https://coliru.stacked-crooked.com/a/915bff19be8c727e "2.689s")  |
| 100.000  | 100.000  | 1.000  | [2.690s](https://coliru.stacked-crooked.com/a/c4210c7e2edd85b8 "2.690s")  | [2.849s](https://coliru.stacked-crooked.com/a/7f97daeedc92f94d "2.849s") |
